# The challenge
When I was a freshman in college we were challenged to manually draw a car only using Bézier curves with Python (Matplotlib). The quality of the final plot would determine our grades. The discipline was a gentle introduction to computer graphics with a prominent mathematical approach.

# How we did it
We used GIMP to preview the Bézier curves with all the control points. It gave me the absolute position of the cursor relative to the image, and then I transferred it to the Python code (`.ipynb`). It really demanded time and attention. It's also a bit hard coded in my opinion, but with the knowledge we had at that time, we managed to plot a very decent outlining.

We used Python 3.7 back in those days as the interpreter for Jupyter Lab, but I tested the whole script with Python 3.12 and it still works like a charm.

We thought the radial decorations of the wheels were way too complex to draw one by one. So we tried to create a function to rotate the points and failed. Then we looked up on StackOverflow and found a [solution](https://stackoverflow.com/a/34374437/13787721) by **Mark Dickinson** that does exactly what we wanted. This saved us a lot of time 🙏🏻. Then we used Mark's function to replicate a single **'YY'** pattern symmetrically, given the number of iterations.

There is a little problem with perspective, especially if you look closely at the wheels. There are some angles and deformations due to the camera angle, but we believe it does not compromise the overall appearance.

I was a naive student so the code is a mess, and there are sections mixing Portuguese and English. But the result turned out really good. My professor told me this was the best work he ever saw in that discipline, (and sure!) my friend and I were immensely glad to hear that!

# The result
![Lamborghini Sián FKP37 - Matplotlib](https://github.com/user-attachments/assets/22bb61f8-0244-401d-84e5-b8eff230beaf)

We also learned to manipulate images using NumPy. Then we loaded the image with Matplotlib and lowered its opacity to ensure the curves were matching the picture. Here's an example:  

![Lamborghini com imagem embaixo](https://github.com/user-attachments/assets/2a779ba9-c41d-4add-bf4b-9d3a27b06c2a)

Here is the original image we took for reference:

<img width="1180" height="330" alt="Lamborghini Sian FKP 37 Right Side" src="https://github.com/user-attachments/assets/39b21b6e-a33b-467c-aaa9-12148a1ec7d5" />
