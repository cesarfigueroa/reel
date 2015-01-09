# Reel

Reel is a tiny (~0.5KB, gzipped) JavaScript library for handling video play states. At the moment, it does two things: it pauses the video when the user has either tabbed away from the page or scrolled beyond the video.

## Installation

Install with Bower (`bower install reel`) or manually download the [reel.min.js](reel.min.js) file to your project’s directory.

## Usage

1. Include the library.

  ```html
  <script src="reel.min.js" defer></script>
  ```

2. Add a hook to the video.

  ```html
  <video data-reel="true"></video>
  ```

3. Instantiate the class.

  ```javascript
  new Reel;
  ```

### Configuration

Reel takes two arguments, in the form of an object.

1. `scrollThreshold: 0.9`: Controls how much a user can scroll past the video before it pauses (this should be a number between 0 and 1).
2. `selector: '[data-reel="true"]'`: Sets the CSS selector that targets the video.
