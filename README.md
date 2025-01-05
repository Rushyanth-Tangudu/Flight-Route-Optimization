# Flight-Route-Optimization

Flight Route Optimization
This repository contains a Python program that performs flight route optimization using Dijkstra's algorithm and provides additional functionality such as displaying all possible paths, graph visualization, and flight booking.

## Features
- Find the fastest flight route between two cities.
- Display all possible flight paths with distances and costs.
- Visualize the graph of flights with highlighted shortest paths.
- Book a flight using multiple payment methods.

## Installation and Setup

### 1. Prerequisites
- Python 3.6 or later
- `graphviz` library (Python package)
- Graphviz software (system installation)

### 2. Installing Python Libraries
Install the required Python libraries using pip:
```bash
pip install graphviz
```

### 3. Installing Graphviz Software

#### Windows Installation
1. Download Graphviz from the official website: [Graphviz Download Page](https://graphviz.org/download/).
2. Install the software by running the downloaded installer.
3. Note the installation directory (e.g., `C:\Program Files\Graphviz\bin`).

#### Add Graphviz to PATH
1. Open the Environment Variables settings:
   - Search for "Environment Variables" in the Start menu.
2. Under "System Properties," click **Environment Variables**.
3. Locate the `Path` variable under "System variables" or "User variables."
4. Edit the `Path` variable and add the Graphviz `bin` directory (e.g., `C:\Program Files\Graphviz\bin`).
5. Restart your terminal or IDE.

#### Verify Installation
Run the following command in the Command Prompt to ensure Graphviz is installed correctly:
```bash
dot -V
```
You should see the version of Graphviz displayed.

## Running the Code

1. Clone the repository:
```bash
git clone https://github.com/yourusername/flight-route-optimization.git
cd flight-route-optimization
```

2. Run the Python program:
```bash
python Flight_Route_Optimization.py
```

3. Follow the prompts:
   - Enter the source and destination cities.
   - Choose an option from the menu to display the fastest route, all paths, or visualize the graph.
   - Book a flight using the desired payment method.

## Features Breakdown

### Menu Options

#### Option 1: Display Fastest Flight and Book Flight
- Uses Dijkstra's algorithm to find the fastest route based on flight time.
- Displays the shortest path with total time and cost.

#### Option 2: Display All Possibilities and Book Flight
- Lists all possible paths between the source and destination.
- Displays the total cost and distance for each path.
- Allows selection of a specific path for booking.

#### Option 3: Display the Graph
- Visualizes the flight graph using Graphviz.
- Highlights the shortest path in red.

#### Option 4: Exit
- Exits the program.

## Example Input/Output

### Input
```plaintext
Source vertex: Delhi
Destination vertex: Mumbai
```

### Output
#### Fastest Flight
```plaintext
Shortest time: 2.05 hours
Total cost: $5139
Path: Delhi -> Mumbai
```

#### All Possible Flights
```plaintext
Path 1: Delhi -> Mumbai
Total Distance: 2.05 hours
Total Cost: $5139
```

#### Graph
A PNG file `highlighted_flight_graph.png` is generated, showing the flight network with the shortest path highlighted.

## Notes
- Ensure the Graphviz `dot` executable is accessible via the `PATH` variable before running the program.
- The program dynamically generates the flight graph and allows real-time interaction for flight selection and booking.

## License
This project is licensed under the MIT License.

## Contribution
Feel free to fork the repository and submit pull requests for improvements or additional features.

