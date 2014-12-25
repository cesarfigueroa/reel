# Reel

Reel is a tiny (534B, gzipped) JavaScript library for handling video play states. At the moment, it does two things: autoplays the video above a specified width (by default, this is 480px) and pauses the video when either the user has tabbed away from the page or scrolled beyond the video.

## Usage

1. Include the library.

  ```html
  <script src="reel.min.js" defer></script>
  ```

2. Add a hook to the video.

  ```html
  <video class="hero-video"></video>
  ```

3. Instantiate the class.

  ```javascript
  new Reel;
  ```

### Configuration

Reel takes three arguments, in the form of an object.

1. `breakpointWidth: 480`: Sets the maximum width at which autoplay is disabled.
2. `scrollThreshold: 0.9`: Controls how much a user can scroll past the video before it pauses (this should be a number between 0 and 1).
3. `selector: '.hero-video'`: Sets the CSS selector that targets the video.
