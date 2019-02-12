# Real-time Illumination for Large Number of Point Light Sources Based on Physics
The main contribution of this project is to propose a new illumination algorithm, which can quickly achieve the illumination for large number of point light sources based on physics.

For the Dragon model, when there are 100 point light sources in the scene, using our algorithm and using GGX BRDF, the results are as follows:
<table>
    <tr>
      <td ><center><img src="https://github.com/ElayDJ/DemoDisplay/blob/master/PlentyLightResult/Our_alpha_0_25.png"  >(a) Our,α=0.25</center></td>
        <td ><center><img src="https://github.com/ElayDJ/DemoDisplay/blob/master/PlentyLightResult/BRDF_alpha_0_25.png"  >(b) GGX BRDF,α=0.25</center></td>
    </tr>
    <tr>
        <td><center><img src="https://github.com/ElayDJ/DemoDisplay/blob/master/PlentyLightResult/Our_alpha_0_5.png"  >(c)Our,α=0.5</center></td>
        <td ><center><img src="https://github.com/ElayDJ/DemoDisplay/blob/master/PlentyLightResult/BRDF_alpha_0_5.png"  >(d)GGX BRDF,α=0.5</td>
    </tr>
    <tr>
        <td><center><img src="https://github.com/ElayDJ/DemoDisplay/blob/master/PlentyLightResult/Our_alpha_0_75.png"  >(e)Our,α=0.75</center></td>
        <td ><center><img src="https://github.com/ElayDJ/DemoDisplay/blob/master/PlentyLightResult/BRDF_alpha_0_75.png"  >(f)GGX BRDF,α=0.75</td>
    </tr>
  <tr>
        <td><center><img src="https://github.com/ElayDJ/DemoDisplay/blob/master/PlentyLightResult/Our_alpha_1_0.png"  >(g)Our,α=1.0</center></td>
        <td ><center><img src="https://github.com/ElayDJ/DemoDisplay/blob/master/PlentyLightResult/BRDF_alpha_1_0.png"  >(h)GGX BRDF,α=1.0</td>
    </tr>
</table>

For the Sponza  model, when there are 100 point light sources in the scene, using our algorithm and using GGX BRDF, the results are as follows:
![Our result](https://github.com/ElayDJ/DemoDisplay/blob/master/PlentyLightResult/OurResult_MS_16.jpg)

(a)Our result for sponza

![GGX BRDF Result](https://github.com/ElayDJ/DemoDisplay/blob/master/PlentyLightResult/BRDFResult_MS_16.jpg)

(b)GGX BRDF result for sponza

And for Sponza model, when rendering different numbers of light sources, the frame rates of BRDF and our algorithm are shown in the table below.

\  | 100 lights| 500 lights | 1000 lights | 5000 lights
:- | :-: | :-: | :-: | :-:
fps of GGX BRDF(fps) | 118 | 23 | 12 | 2
fps of our algorithm(fps) | 285 | 56 | 28 | 5
saved rendering time(ms) | 4.97 | 25.62 | 47.62 | 255.49

[Reference]: This paper is in the process of publication.

# Ocean Simulation Based on Geometry Clipmap
The main contribution of this project is to propose to apply the Geometry Clipmap technique used in terrian rendering to large-scale ocean rendering. And some adjustments and improvements are made to fit dynamic ocean scene better. The rendering results are shown below.
![](https://github.com/ElayDJ/DemoDisplay/blob/master/OceanResult/Ocean.png)
The corresponding ocean grid is shown below.
![](https://github.com/ElayDJ/DemoDisplay/blob/master/OceanResult/Mesh.png)
When the number of grid LOD layers changes, the corresponding rendering frame rate and memory consumption are shown in the following table.

Number of lod layers   | 2 | 5 | 7 | 10
:- | :-: | :-: | :-: | :-:
Frame rate(fps) | 1847 | 1720 | 1563 | 1476
CPU memory(M) | 40 | 40 | 40 | 41
GPU memory(M) | 29 | 30 | 30 | 31

[Reference]: Asirvatham A, Hoppe H. Terrian rendering using GPU-based geometry clipmaps[J]. Gpu Gems, 2005.

# Tiled Forward Shading
The main work of this project is to use screen space partitioning to eliminate light sources and achieve a large number of point light sources rendering based on Phong model. And I design and implement three rendering frameworks: forward shading, deffered shading and tiled shading. The final tiled shading results are shown below.
![](https://github.com/ElayDJ/DemoDisplay/blob/master/TiledShadingResult/TileShading.png)
At the same light source density, the frame rates of forward shading, deferred shading and tiled forward shading are compared as follows.
![](https://github.com/ElayDJ/DemoDisplay/blob/master/TiledShadingResult/FrameRateCompare1.png)

[Reference]: Billeter M , Olsson O , Assarsson U . Tiled Forward Shading[J]. 2013.

# Forward Light Cut
The main work of this project is to simulate secondary reflection by generating a large number of virtual point light sources on the triangular surface of the model. The rendering results are shown below.
![](https://github.com/ElayDJ/DemoDisplay/blob/master/FLCResult/FLCCornelBoxResult.png)
The corresponding rendering frame rate is 284 fps.

# Real-Time Polygonal-Light Shading with Linearly Transformed Cosines 
The main work of this project is to approximate the BDRF integral of the polygonal light source by cosine integral of the polygon on the sphere. The rendering results are shown below.
![](https://github.com/ElayDJ/DemoDisplay/blob/master/PolygonalLightResult/UniformPolygonalLightResult.png)
![](https://github.com/ElayDJ/DemoDisplay/blob/master/PolygonalLightResult/TexturedPolygonalLightResult.png)

# Dynamic Image Based Lighting
The main work of this project is: inspired by the idea of polygon light source, filter light source texture dynamically to approximate the illumination effect of dynamic scenes on objects. The rendering results are shown below.
![]()

# Particle Effects Using Compute Shader
The main work of this project is to use compute shaders and imge buffers to achieve dynamic movement, generation and destruction of particle effects. The rendering results are shown below. The number of particles is about **10 million**. The corresponding rendering frame rate is 12 fps.
![](https://github.com/ElayDJ/DemoDisplay/blob/master/ParticleResults/Particle.png)
![](https://github.com/ElayDJ/DemoDisplay/blob/master/ParticleResults/Particle3.png)

# MiniGame Demo(GAD, Tencent)
This is a 3D cool run mini game, similar to temple run. Game screenshots are as follows.
![](https://github.com/ElayDJ/DemoDisplay/blob/master/GADDemo/MiniGame2.png)
