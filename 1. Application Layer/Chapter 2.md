# 2.6 Video Streaming and Content Distribution Networks

## 2.6.2 HTTP Streaming & DASH
1. HTTP STREAMING
	- **Storage and Access**: Video is stored on an HTTP server as a regular file with a specific URL.
	- **Client Request**: The client establishes a TCP connection and sends an HTTP GET request for the video URL.
	- **Data Transfer**: The server responds with the video file, transmitting data as quickly as network conditions permit.
	- **Buffering and Playback**:
	    - The client collects incoming bytes in a buffer.
	    - Playback begins once the buffer reaches a predetermined threshold.
	    - The application decompresses frames from the buffer and displays them.
	- **Limitation**:
	    - All clients receive the same video encoding.
	    - Does not account for varying bandwidth among different clients or over time.
1. Dynamic Adaptive Streaming over HTTP (DASH)
	- **Multiple Encodings**: Video is encoded in several versions at different bit rates and quality levels.
	- **Chunk-Based Requests**:
	    - Video is divided into segments of a few seconds each.
	    - Clients request chunks one at a time using HTTP GET requests.
	- **Adaptive Streaming**:
	    - Clients select chunks based on current bandwidth conditions.
	    - High bandwidth: select high-rate (high-quality) chunks.
	    - Low bandwidth: select low-rate (lower-quality) chunks.
	- **Manifest File**:
	    - Stored on the server with URLs and bit rates for each video version.
	    - Clients request the manifest file to learn about available versions.
	- **Bandwidth Measurement**:
	    - Clients measure received bandwidth during downloads.
	    - Use a rate determination algorithm to decide the quality of the next chunk.
	- **Advantages**:
	    - Accommodates clients with varying internet speeds.
	    - Adapts to bandwidth fluctuations during a session.
	    - Essential for mobile users with changing network conditions.
	    - Allows seamless switching between different quality levels.


## 2.6.3 Content Distribution Networks (Streaming)
