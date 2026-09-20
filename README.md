Time Complexity Visualizer
Description

This project is a Flask application that measures the running time of different algorithms and generates graphs to visualize their time complexity.

The application supports:

Linear Search
Bubble Sort
Binary Search
Nested Loops
Insertion Sort
Selection Sort

The generated graphs are saved locally, and the image is also returned as a Base64-encoded string in the JSON response.

Technologies
Python
Flask
Matplotlib
How to Run

Install the required libraries:

pip install flask matplotlib

Run the application:

python app.py

The server runs at:

http://localhost:8000
API Usage

Use the /analyze endpoint with:

algo - algorithm name
step - input size step
n_max - maximum input size

Example:

http://localhost:8000/analyze?algo=linear_search&step=10&n_max=10000

Other examples:

http://localhost:8000/analyze?algo=bubble_sort&step=10&n_max=1000
http://localhost:8000/analyze?algo=binary_search&step=10&n_max=10000
http://localhost:8000/analyze?algo=nested_loops&step=10&n_max=1000
Generated Graphs

Graphs are saved in the snapshots folder as PNG files.

Example:

snapshots/linear_search.png

The API response contains the input sizes, execution times, image path, and Base64-encoded image.
