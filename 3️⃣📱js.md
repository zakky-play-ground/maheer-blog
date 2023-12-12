To make your React Three Fiber (R3F) application responsive and interactive across all devices, including mobile, you need to consider a few key aspects:

1. **Responsive Design**: Ensure your application is responsive to different screen sizes. This can be achieved by setting the width and height of the `Canvas` component to fit the parent node. The `Canvas` component is responsive by default, so you just need to control the size of its parent node [Source 2](https://docs.pmnd.rs/react-three-fiber/getting-started/your-first-scene).

```jsx
<div id="canvas-container">
 <Canvas />
</div>
```

2. **Touch Events**: R3F supports touch events out of the box. You can use the same event handlers (`onPointerDown`, `onPointerUp`, `onPointerOver`, `onPointerOut`, `onPointerMove`) for both mouse and touch events. This means you can use the same code for both desktop and mobile devices [Source 0](https://docs.pmnd.rs/react-three-fiber/getting-started/introduction).

3. **Orbit Controls**: To make the 3D scene interactive on mobile devices, you can use the `OrbitControls` component from `@react-three/drei`. This component allows users to orbit around the scene using touch controls [Source 3](https://blog.salvatorelabs.com/building-immersive-web-apps-a-guide-to-creating-interactive-experiences-with-react-three-and-fiber-r3f/).

```jsx
import { OrbitControls } from '@react-three/drei'

function App() {
 return (
   <Canvas>
     <OrbitControls />
     {/* Your models go here */}
   </Canvas>
 )
}
```

4. **Animations**: Animations can be used to create interactive experiences. For example, you can animate the rotation of your 3D models using the `useFrame` hook in R3F. This hook allows you to run a function on every frame, which can be used to animate your models [Source 3](https://blog.salvatorelabs.com/building-immersive-web-apps-a-guide-to-creating-interactive-experiences-with-react-three-and-fiber-r3f/).

```jsx
useFrame((state, delta) => (meshRef.current.rotation.x += delta))
```

5. **Performance**: Performance is crucial on mobile devices. Make sure to optimize your models and animations to ensure a smooth user experience. You can use tools like `@gltf-transform/cli` to reduce the size of your 3D models [Source 3](https://blog.salvatorelabs.com/building-immersive-web-apps-a-guide-to-creating-interactive-experiences-with-react-three-and-fiber-r3f/).

By following these steps, you can create an interactive R3F application that works well on both desktop and mobile devices.