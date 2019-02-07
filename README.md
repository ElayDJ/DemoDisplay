# Real-time illumination for large number of point light sources based on physics
The main contribution of this project is to propose a new illumination algorithm, which can quickly achieve the illumination for large number of point light sources based on physics.

For the Dragon model, when there are 100 point light sources in the scene, using our algorithm and using GGX BRDF, the results are as follows:
<div align="center">
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
</div>

  <center>
  are
  </center>
