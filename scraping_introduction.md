
# PLOTLY INTRODUCTION


    import plotly.plotly as py
    from plotly.graph_objs import *

### CONVERTING PLOTLY IMAGE TO MARKDOWN FORMAT


    import matplotlib.pyplot as plt
    import numpy as np
    import plotly.plotly as py
    
    n = 50
    x, y, z, s, ew = np.random.rand(5, n)
    c, ec = np.random.rand(2, n, 4)
    area_scale, width_scale = 500, 5
    
    fig, ax = plt.subplots()
    sc = ax.scatter(x, y, c=c,
                    s=np.square(s)*area_scale,
                    edgecolor=ec,
                    linewidth=ew*width_scale)
    ax.grid()
    
    py.iplot_mpl(fig)




<iframe id="igraph" scrolling="no" style="border:none;"seamless="seamless" src="https://plot.ly/~kpadmana/527.embed" height="525px" width="100%"></iframe>




    import plotly.tools as tls
    
    tls.embed("https://plot.ly/~streaming-demos/4")




<iframe id="igraph" scrolling="no" style="border:none;"seamless="seamless" src="https://plot.ly/~streaming-demos/4.embed" height="525" width="100%"></iframe>




    
