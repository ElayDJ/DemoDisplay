# Real-time illumination for large number of point light sources based on physics
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

 1  | 100 lights| 500 lights | 1000 lights | 5000 lights
:- | :-: | :-: | :-: | :-:
fps of GGX BRDF(fps) | 118 | 23 | 12 | 2
fps of our algorithm(fps) | 285 | 56 | 28 | 5
saved rendering time(ms) | 4.97 | 25.62 | 47.62 | 255.49

