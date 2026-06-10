# JupyterLab4.github.io
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mastering JupyterLab</title>
    <style>
        /* Modern Reset & Variables */
        * {
            margin: 0;
            padding: 0;
            box-box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        :root {
            --bg-color: #0f172a;
            --card-bg: #1e293b;
            --accent-orange: #f97316;
            --accent-blue: #38bdf8;
            --text-main: #f8fafc;
            --text-muted: #94a3b8;
        }

        body {
            background-color:#cc4e00;
            color: var(--text-main);
            line-height: 1.6;
        }

        /* Navbar */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.5rem 10%;
            background-color:rgb(180, 60, 0);
            backdrop-filter: blur(10px);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--text-main);
        }
        .logo span {
            color: var(--accent-orange);
        }
        .nav-links a {
            color: var(--text-muted);
            text-decoration: none;
            margin-left: 2rem;
            transition: color 0.3s;
        }
        .nav-links a:hover {
            color: var(--accent-blue);
        }

        /* Hero Section */
        .hero {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 5rem 10%;
            min-height: 80vh;
        }
       
        .hero-content, [class*="hero"] {
            width: 100% !important;
            max-width: 950px !important; 
            margin: 0 auto !important;  
            padding: 40px 20px !important;
            text-align: left !important;  
        }
        .hero-content h1 {
            font-size: 3.5rem;
            line-height: 1.2;
            margin-bottom: 1.5rem;
        }

       .hero-content h1 span {
            color: var(--accent-orange);
        }
        .hero-content p {
            font-size: 1.2rem;
            color: var(--text-muted);
            margin-bottom: 2rem;
            max-width: 800px; 
        }
         .btn {
            display: inline-block;
            background: linear-gradient(135deg, var(--accent-orange), #ea580c);
            color: white;
            padding: 0.8rem 2rem;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 20px rgba(249, 115, 22, 0.4);
        }
        /* Interactive Code Box Demo */
        .hero-visual {
            max-width: 45%;
            width: 100%;
        }
        .code-box {
            background-color:#cc4e00;
            border-radius: 8px;
            padding: 1.5rem;
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
            border: 1px solid #334155;
        }
        .code-header {
            display: flex;
            gap: 0.5rem;
            margin-bottom: 1rem;
        }
        
        .code-input {
            color:#cc4e00 ;
            font-family: 'Courier New', Courier, monospace;
            margin-bottom: 1rem;
        }
        .code-output {
            background-color: #0f172a;
            padding: 1rem;
            border-radius: 4px;
            border-left: 4px solid var(--accent-orange);
            font-family: monospace;
        }

        /* Curriculum Section */
        .curriculum {
            padding: 5rem 10%;
            background-color: #0b111e;
        }
        .curriculum h2 {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
        }
       .grid,.row, [class*="card-container"], [class*="wrapper"]{
            display:flex !important;
            flex-direction: column !important;
            align-items: center !important;
             width: 100% !important; 
       }
      .card,[class*="box"], [class*="item"]{
            background-color: var(--card-bg);
            width: 100% !important;
            max-width: 800px !important;
            margin-bottom: 24px !important; 
            padding: 24px !important;
       }
        .card:hover {
            transform: translateY(-5px);
        }
        .card h3 {
            color: var(--accent-orange);
            margin-bottom: 1rem;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2rem;
            color: var(--text-muted);
            border-top: 1px solid #1e293b;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .hero {
                flex-direction: column;
                text-align: center;
                padding-top: 2rem;
            }
            .hero-content {
                max-width: 100%;
                margin-bottom: 3rem;
            }
            .hero-visual {
                max-width: 100%;
            }
            .nav-links {
                display: none; /* Keep it simple for mobile */
            }
        }
    </style>
</head>
<body>
    <nav>
        <div class="logo">🚀 Learn<span>Jupyter</span></div>
    </nav>

    <section class="hero">
        <div class="hero-content">
             <a href="https://ayana-sarkar.github.io/Home2.github.io/" class="btn">Basics</a>
             <a href="https://ayana-sarkar.github.io/JupyterLab4.github.io/" class="btn">Plotting with List</a>
            <a href="https://ayana-sarkar.github.io/JupyterLab5.github.io/" class="btn">Plotting with Arrays</a>
            <a href="https://ayana-sarkar.github.io/JupyterLab2.github.io/" class="btn">Interpolation</a>
            <a href="https://ayana-sarkar.github.io/JupyterLab1.github.io/" class="btn">Special func</a>
            <a href="https://ayana-sarkar.github.io/JupyterLab3.github.io/" class="btn">Let's Practice more!</a>
            <h1>Plotting with<span>Lists</span></h1>
            <p>A list is used to store an ordered collection of items in a single variable.A list is defined by placing items inside square brackets [], separated by commas.Items can be change, add, or remove from a list.Lists can have multiple items with the same value (e.g., [1, 2, 2, 3]). Plotting with lists in JupyterLab is incredibly straightforward, usually done using the Matplotlib library (specifically the pyplot module).</p>
            </div>
        </section>

    <section id="curriculum" class="curriculum" style="background-color: #cc4e00;">
            <div class="card">
                <h2>1.Scatter Plot</h2>
                <img src="Screenshot 2026-06-09 150323.png" alt="Data Visualization" class="box-image">
                <p>
                Line1: This imports the pyplot module from the matplotlib library, which is the standard tool for creating visualizations in Python.<br>
                Line2,3:These two lines create Python lists containing your data points.Matplotlib maps these lists together by index. For example, the first data point plotted on the graph is at coordinates (5, 99), the second is at (7, 86), the third is at (8, 87), and so on.<br>
                Line4: This tells Matplotlib to generate a scatter plot using your data.<br>
                x and y tell it which data to use for the horizontal and vertical axes.<br>
                color='purple' changes the default blue dots to purple.<br>
                Line5 :This adds the text "Age vs. Speed" right above the top center of the plot box so viewers know what the chart represents.<br>
                Line6: This tells Python to finalize the figure and cleanly render it on your screen .It cleanly closes the plot object in the background and prevents annoying text summaries (like <matplotlib.collections.PathCollection at 0x... >)</p>
                </div>
            <div class="card">
                <h2>2.Sine Function</h2>
                <img src="Screenshot 2026-06-06 001335.png" alt="Data Visualization" class="box-image">
                <p>Lines 1: This brings in Python's premier plotting library.<br> 

               Line2: This extracts the specific math components needed for a sine wave:<br> 
               Lines 4–5: A plot needs data points (x, y) to draw a line. These lines use list comprehensions (shorthand loops) to generate 200 distinct coordinate points.                <br> 
             [Range(200) means i has values from 0 to 199]<br> 
              Line 7: The Core Plotting Command<br> 
                 This is the command that actually builds the graph in the background.<br> 
                x, y: Tells it what coordinates to map.<br> 
            'r-': A formatting shortcut meaning red - solid line.<br> 
            label='sin(x)': Attaches a name tag to this specific line (crucial for the legend later).<br> 
             linewidth=2: Makes the line thicker and easier to read.<br> 
             Lines 8–9: Labels the horizontal and vertical axes so the viewer knows what the scales represents.<br> 
               Line10: Adds a prominent title at the very top of the graph to declare what the entire visual represents.<br> 
              Line11: Draws gridlines (horizontal and vertical intersection lines) in the background.<br> 
               Line12: Searches the graph for any label properties (defined back in Line 7) and draws a little legend box in the corner, confirming that the red line represents sin(x).<br> 
               Line13: This command makes Matplotlib to take everything it built in the background and pop it up cleanly on your screen.The green part is just a comment that does not contribute to the graph.<br></p>
               <img src="Screenshot 2026-02-27 171437.png" alt="Data Visualization" class="box-image">
            </div>
            <div class="card">
                <h2>3. Multiple curves</h2>
                 <img src="Screenshot 2026-02-27 171547.png" alt="Data Visualization" class="box-image">
                <p>When plt.plot(...) is called for the first time in a cell (Line 5), Matplotlib initializes a new figure and a set of axes (the canvas). It  draws the first line (y1) onto it.Next, when plt.plot(...) is called a second time immediately after (Line 6), Matplotlib doesn't erase what it just did. Instead, it layers the new data directly on top of the existing canvas.<br> 

                Line5: This takes the list of horizontal coordinates (x) and your first list of vertical coordinates (y1). It plots a linear straight line (y = x) . It assigns a name tag (label='y = x') to this specific line so the legend can identify it later.<br> 

                Line6: Does the exact same thing-- This takes the same horizontal coordinates (x) but pairs them with your second list of vertical coordinates (y2). It gives this second line its own distinct name tag (label='y = x^2').<br></p>
            </div>
            <div class="card">
                <h2>4.Lets Plot the function f(x) = exp(−x) cos(2πx) for x ∈ [0, 5] using list comprehension</h2>
                <img src="Screenshot 2026-02-08 102726.png" alt="Data Visualization" class="box-image">
                <p>Line1: Matplotlib.pyplot is imported so that plt functions can be used<br> 
                 Line2: Cos ,Pi, exponential are needed for the plot, so they are also imported.<br>  
                 Line3: Here only 5 five values are taken for x (0,1,2,3,4). That’s why the curve not smooth.<br> 
                Line4: the function is defined.<br>
                Line5: x and y axes respectively, represent the x and corresponding f values. A red-solid line is used, and the curve is labelled as f(x).<br> </p>
            </div>
            <div class="card">
                <h2>5.Plot cos(x) and sin(x) in the same figure for x ∈ [0, 2π] </h2>
                 <img src="Screenshot 2026-02-08 110932.png" alt="Data Visualization" class="box-image">
                <p>Line3: Range for x is taken from 0 to 62. This is a large number of points , so the graph is much smoother. The reason we kept the range till 62 because, it is important to take values of x from 0 to 2Pi (3.14 * 2=6.2)<br>
                plt.legend made the little legend box pop in the corner, denoting the sinx and cosx lines.</p>
            </div>
            <div class="card">
                <h2>6.Using “linspace"</h2>
                 <img src="Screenshot 2026-02-08 112716.png" alt="Data Visualization" class="box-image">
                 <p>Line1-2: Numpy and MatplotLib are both imported here for computing.And the statements as np and as plt create aliases (shortcuts). <br> 
                    np tells Python: "Look inside the NumPy library." (e.g., np.sin() or np.linspace())<br>          
                    plt tells Python: "Look inside the Matplotlib plotting module." (e.g., plt.plot() or plt.grid())<br> 
                    Line3: The linspace Command:<br> 
                    np.linspace creates a NumPy array, which functionally acts as a mathematical vector. np.linspace stands for "linear space". So, tvec becomes an array containing 100 numbers, starting exactly at 0, ending exactly at 10, all spaced perfectly apart (0, 0.101, 0.202, ... up to 10). It even includes the value 10 unlike range( ) .<br> 
                    Computers cannot actually draw smooth, continuous mathematical curves. Instead, they cheat by plotting a lot of tiny, individual straight lines between points so closely packed together that they look like a smooth curve to the human eye. By using 100 points, the sine waves look beautifully smooth. linspace is  useful because there is no need to figure out the exact decimal step size . <br> </p>
        </div>
    </section>
    <footer>
        <a href="https://ayana-sarkar.github.io/Home2.github.io/" class="btn">Previous</a>
        <a href="https://ayana-sarkar.github.io/JupyterLab5.github.io/" class="btn">Next</a>
</body>
</html>
