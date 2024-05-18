# Instagram Videos Downloader

Simple Website/API for downloading instagram videos made with Next.js that actually works with no problem.

## Description

A website that lets you download Instagram videos easily and quickly. You can paste the URL of any public Instagram post and get the video file in MP4 format. there is also an API that you can use to integrate this functionality into your own applications. The API is simple, and it returns JSON responses with the video URL and other metadata.

_Note: Instagram stories aren't supported._


## Getting Started

**1.** Cloning the repository:

```bash
git clone https://github.com/ironmercdanish.git
```

**2.** Installing dependencies:

```bash
cd instagram-video-downloader
```

```bash
npm install
```

**3.** Starting the server:

```bash
# Development
npm run dev

# Build
npm run build

# Start
npm run start
```

### Endpoint: /api/video?postUrl={POST_URL}

Parameters :

- `postUrl` : Instagram Post or Reel link **(required)**.

#### GET Request example

```bash
curl -i "http://localhost:3000/api/video?postUrl=https://www.instagram.com/p/CGh4a0iASGS"
```

#### API Response

```json
{
  "status":"success",
  "data":
    {
      "filename":"ig-downloader-1712666263.mp4",
      "width":"640",
      "height":"640",
      "videoUrl":"https://scontent.cdninstagram.com/o1/v/t16/f1/m84/E84E5DFC48EA8...etc"
    }
}
```

