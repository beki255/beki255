<h1 align="center">Hi 👋, I'm Bereket</h1>
<h3 align="center">A passionate full stack developer from ethiopia</h3>
<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
     
<script src="https://cdn.jsdelivr.net/npm/three@0.145/build/three.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/three@0.145/examples/js/controls/OrbitControls.js"></script>

    </head>
    <body>
        
    </body>
<script>
//import * as THREE from 'three';
//import { OrbitControls } from 'three/examples/jsm/controls/OrbitControls';

let cw=400

let ch=700

const scene=new THREE.Scene();

const camera=new THREE.PerspectiveCamera(75,cw/ch,0.1,1000);

camera.position.z=2

const renderer=new THREE.WebGLRenderer();
document.body.appendChild(renderer.domElement)

renderer.setSize(cw,ch)

renderer.setPixelRatio(devicePixelRatio)


//const orbitcontrols=new THREE.OrbitControls(camera,renderer.domElement)

//orbitcontrols.enableDamping=true


//orbitcontrols.dampingFactor=0.01



//allcomponents

var vec1= new THREE.Vector3(6,6,8)
var vec2= new THREE.Vector3(1,1,1)
var vec3=vec1.clone().add(vec2) 
//console.log(vec1.z)





let geo=new THREE.TorusGeometry(2,.3,16,100) 



let material=new  THREE.MeshStandardMaterial({color:0xfffff,

wireframe:true
})


let m2=new THREE.MeshStandardMaterial({color:0xccff,
flatShading:true,

})


let mesh=new THREE.Mesh(geo,material)

let sp=new THREE.IcosahedronGeometry(.02,2)

let spm=new THREE.Mesh(sp,m2)


const light=new THREE.HemisphereLight(0xFF6347,0x00BFFF,1)

let axes=new THREE.AxesHelper(200)
//scene.add(axes)
scene.add(mesh)
scene.add(spm)
scene.add(light)
let t=0
//scene.scale.set(5)
function animate(){

requestAnimationFrame(animate)

renderer.render(scene,camera)

//orbitcontrols.update()

let rad=2

let pos=new THREE.Vector3(rad*Math.cos(t),rad*Math.sin(t),0)
let pos2=new THREE.Vector3(rad*Math.cos(t+0.1),rad*Math.sin(t+0.1),0)



let axis = new THREE.Vector3(1, 1, 1); // Z-axis

// Define the angle of rotation (90 degrees in radians)
let angle = Math.PI/2; // 90 degrees = π/2 radians

// Rotate the vector






let n=pos2.clone().sub(pos).normalize()

n.applyAxisAngle(axis, angle).normalize();


camera.up.set(n.x,n.y,n.z)
//camera.position.set(x,y,0); // Move the camera

//scene.rotation.z=t
//scene.rotation.x=Math.PI/2
//scene.scale.set(1)
spm.position.set(pos.x,pos.y,pos.z)


camera.position.set(pos2.x,pos2.y,pos2.z)

camera.lookAt(pos)
//camera.lookAt(scene.position)


t-=0.01

camera.updateProjectionMatrix()

}
animate()
</script>
</html>

- 🌱 I’m currently learning **Computer science**

- 💬 Ask me about **C++ and python**

- 📫 How to reach me **Bereket2553@gmail.com**

- ⚡ Fun fact **I think i am happy**

<h3 align="left">Connect with me:</h3>
<p align="left">
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://www.cprogramming.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="c" width="40" height="40"/> </a> <a href="https://clojure.org/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/5/5d/Clojure_logo.svg" alt="clojure" width="40" height="40"/> </a> <a href="https://www.cockroachlabs.com/product/cockroachdb/" target="_blank" rel="noreferrer"> <img src="https://cdn.worldvectorlogo.com/logos/cockroachdb.svg" alt="cockroachdb" width="40" height="40"/> </a> <a href="https://www.w3schools.com/cpp/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="cplusplus" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://ifttt.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/ifttt/ifttt-ar21.svg" alt="ifttt" width="40" height="40"/> </a> <a href="https://www.java.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="40" height="40"/> </a> <a href="https://www.linux.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> <a href="https://www.oracle.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/oracle/oracle-original.svg" alt="oracle" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://developer.apple.com/swift/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/swift/swift-original.svg" alt="swift" width="40" height="40"/> </a> </p>

<p>&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=beki255&show_icons=true&locale=en" alt="beki255" /></p>
