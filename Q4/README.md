# Two Body Simulation
So I have solved the question differently using two facts:
1) Keplers Second Law: $$\frac{1}{2}r^2\frac{d\theta}{dt} = \frac{\pi ab}{P}$$
where $P$ is the time period and $a$ and $b$ are major and minor axes.
2) Polar Equation of Ellipse:
$$r = \frac{a(1-e^2)}{1 + ecos\theta}$$

Therefore I found coordinates of planet through $rcos\theta$ and $rsin\theta$. After every timefame, I incremented the value of $\theta$ by $d\theta$ calculated from the above formula by assuming $dt$ to some value.Then I updated the value of $r$ in each iteration to get the position of the planet at any time.
