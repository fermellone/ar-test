<!-- minimal loader shown until image descriptors are loaded -->
<div class="arjs-loader">
  <div>Loading, please wait...</div>
</div>
<a-scene
  vr-mode-ui="enabled: true;"
  renderer="logarithmicDepthBuffer: true;"
  embedded
  arjs="trackingMethod: best; sourceType: webcam; debugUIEnabled: true;"
>
  <!-- use rawgithack to retrieve the correct url for nft marker (see 'trex' below) -->
  <a-nft
    type="nft"
    url="https://arjs-cors-proxy.herokuapp.com/https://raw.githack.com/AR-js-org/AR.js/master/aframe/examples/image-tracking/nft/trex/trex-image/trex"
    smooth="true"
    smoothCount="10"
    smoothTolerance="0.01"
    smoothThreshold="5"
  >
    <a-entity
      gltf-model="https://arjs-cors-proxy.herokuapp.com/https://raw.githack.com/AR-js-org/AR.js/master/aframe/examples/image-tracking/nft/trex/scene.gltf"
      scale="5 5 5"
      position="100 100 0"
    />
  </a-nft>
  <a-entity camera />
</a-scene>
