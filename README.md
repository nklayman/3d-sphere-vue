# 3D Sphere Vue

Renders a large number of 3D cubes with [Three.js](https://threejs.org/) and WebGl, demoing Vue's performance with a large number of components and rapidly updating data. However, this should not be used as a performance benchmark.

## Examples:

### Rendered in Vanilla JS, wrapped with Vue:

[Vue 2](https://3d-sphere-vue.nklayman.now.sh/vue2.html)

[Vue 3](https://3d-sphere-vue.nklayman.now.sh/vue3.html)

These examples use pure js to control the rendering of the cubes, they are only wrapped in a Vue component. Therefore, Vue 2 and 3 have the same performance. This is practically the same as not using Vue at all, so especially don't use this as a benchmark.

### Each cube controlled by a Vue component

[Vue 2](https://3d-sphere-vue.nklayman.now.sh/vue2ComponentBoxes.html)

[Vue 3](https://3d-sphere-vue.nklayman.now.sh/vue3ComponentBoxes.html)

In these examples, each cube is controlled by its own Vue component. A parent component gives the children components new orientation (via props), and the children components then update the Three.js mesh. In this scenario, Vue 3 has better performance as all the updates have to go through Vue's reactivity system.

## Other links:

[Twitter thread of original React demo](https://twitter.com/0xca0a/status/1199997552466288641)

[Twitter thread of original Vue demo](https://twitter.com/igorhalfeld/status/1201161977973882880) - All of these examples were derived from this, shoutout to @igorhalfeld. The Vue 2 vanilla demo is effectively the same code as this.
