Here’s a 9-step process:
  1. The user creates a video upload request and provides the video files along with the details about the video.
  1. The raw video files are uploaded to an Object Storage (such as S3).
  1. Also, the metadata is saved in a database as well as a cache for faster retrieval when needed.
  1. The raw video files are sent for transcoding to a special transcoding server. Transcoding is the process of encoding the videos into compatible bitrates and formats for streaming.
  1. The transcoded video is uploaded to another object storage.
  1. The notification for transcoding completion is sent to a special service via a message queue.
  1. The Transcoding Status Handler updates the metadata DB and cache with the latest details of the video.
  1. The user raises a video streaming request that goes to a Content Delivery Network (CDN).
  1. The CDN fetches the video from the object storage for streaming. It also caches the video locally for subsequent streaming requests.

<img src="https://substack-post-media.s3.amazonaws.com/public/images/5237f88e-8a2c-4e0b-8457-3dfabd2d6ca3_1329x1536.gif">
