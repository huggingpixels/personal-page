  <script>
    export let delayTime = Math.floor(Math.random() * Math.floor(15)) +'s';
    export let randomSize = Math.floor(Math.random() * (+200 - +80) + +80);
    export let randomPlaceX = Math.floor(Math.random() * Math.floor(200)) + 'px';
    export let randomPlaceY = Math.floor(Math.random() * Math.floor(400)) + 'px';
  </script>

<style>
#cloud {
	transform: translate(0px, 0px);
  animation: float 8s ease-in-out infinite;
  position: absolute;
  }
  
  @keyframes float {
	0% {
		transform: translate(0px, 0px);
	}
	50% {
		transform: translate(5px, -15px);
	}
	100% {
		transform: translate(0px, 0px);
	}
}
  </style>

  <svg
    xmlns="http://www.w3.org/2000/svg"
    xmlns:xlink="http://www.w3.org/1999/xlink"
    id="cloud"
    version="1.1"
    width={randomSize}
    viewBox="0, 0, 400,271"
    style="animation-delay: {delayTime};
    top: {randomPlaceX};
    left: {randomPlaceY}">
    <g id="svgg">
      <path
        id="path0"
        d="M203.155 5.783 C 180.817 12.033,160.533 28.287,149.785 48.548 C
        142.735 61.837,139.882 62.983,132.941 55.315 C 109.792 29.735,55.263
        64.138,55.263 104.324 C 55.263 107.881,52.843 111.622,49.342 113.474 C
        -1.959 140.622,-11.757 216.515,31.451 252.057 L 41.949 260.692 200.022
        260.762 C 375.952 260.839,363.882 262.020,382.082 242.947 C 414.178
        209.312,401.903 139.913,359.852 117.267 C 351.275 112.647,350.587
        111.296,349.179 96.296 C 342.899 29.403,273.182 -13.811,203.155 5.783 "
        stroke="none"
        fill="#fcfcfc"
        fill-rule="evenodd" />
      <g xmlns="http://www.w3.org/2000/svg" id="svgg">
        <path
          id="path0"
          d="M203.155 5.783 C 180.817 12.033,160.533 28.287,149.785 48.548 C
          142.735 61.837,139.882 62.983,132.941 55.315 C 109.792 29.735,55.263
          64.138,55.263 104.324 C 55.263 107.881,52.843 111.622,49.342 113.474 C
          -1.959 140.622,-11.757 216.515,31.451 252.057 L 41.949 260.692 200.022
          260.762 C 375.952 260.839,363.882 262.020,382.082 242.947 C 414.178
          209.312,401.903 139.913,359.852 117.267 C 351.275 112.647,350.587
          111.296,349.179 96.296 C 342.899 29.403,273.182 -13.811,203.155 5.783 "
          stroke="none"
          fill="#fcfcfc"
          fill-rule="evenodd" />
      </g>
    </g>
  </svg>