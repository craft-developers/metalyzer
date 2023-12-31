## metalyzer

**metalyzer** is a lightweight JavaScript library for extracting metadata from video/Image files. It provides a simple API to retrieve information such as type, size, dimensions, base64, blob, URL,thumbail,video-duration, and more.

## Installation

```
npm install metalyzer
```

## Usage for Video

```Typescript
const metaData = await extractVideoMetadata(video);
const videoUrl = await extractVideoUrl(video);
const videoBlob = await convertVideoInBlob(video);
console.log(metaData);
console.log(videoUrl);
console.log(videoUrl);
```

## Usage for Image

```Typescript
const metaData = await extractImageMetadata(video);
const imageUrl = await extractImageUrl(video);
const imageBase64 = await extractImagebase64(video);
const [thumbnail1, thumbnail2] = await extractThumbnailFromVideo(video);
console.log(metaData);
console.log(imageUrl);
console.log(imageBase64);
<img src={thumbnail1} />
<img src={thumbnail2} />
```

## Features

- Extracts various video metadata, including file name,url,base64, blobm, dimensions, duration, etc.
- Provides a simple and easy-to-use API for metadata extraction.

## APIs

```Typescript
    extractVideoMetadata(videoFile: File): Promise<VideoMetadata>
    extractImageBase64(imageFile: File): Promise<string>;
    extractImageMetadata(imageFile: File): Promise<ImageMetadata>;
    extractImageUrl(imageFile: File): Promise<string>;
    convertVideoInBlob(videoFile: File): Promise<Blob>;
    extractVideoMetadata(videoFile: File): Promise<VideoMetadata>;
    extractVideoUrl(videoFile: File): Promise<string>;
    getFileExtension(fileName: string): string;
    extractThumbnailFromVideo(videoFile: File): Promise<File>
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests to us.

## Issues

If you discover any issues, please [open an issue](https://github.com/your-username/metalyzer/issues).

## Changelog

See the [CHANGELOG.md](CHANGELOG.md) file for details on changes and releases.
