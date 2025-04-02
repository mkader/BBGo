* Live streaming is challenging because the video content is sent over the internet in near real-time. Video processing is compute-intensive. Sending a large volume of video content over the internet takes time. These factors make live streaming challenging.
  1. Step 1: The streamer starts their stream. The source could be any video and audio source wired up to an encoder
  1. Step 2: To provide the best upload condition for the streamer, most live streaming platforms provide point-of-presence servers worldwide. The streamer connects to a point-of-presence server closest to them.
  1. Step 3: The incoming video stream is transcoded to different resolutions, and divided into smaller video segments a few seconds in length.
  1. Step 4: The video segments are packaged into different live streaming formats that video players can understand. The most common live-streaming format is HLS, or HTTP Live Streaming.
  1. Step 5: The resulting HLS manifest and video chunks from the packaging step are cached by the CDN.
  1. Step 6: Finally, the video starts to arrive at the viewer’s video player.
  1. Step 7-8: To support replay, videos can be optionally stored in storage such as Amazon S3.

<img src="https://substack-post-media.s3.amazonaws.com/public/images/e8362079-b1a7-4e39-ac5a-d665ca3b2231_1280x1664.gif">
