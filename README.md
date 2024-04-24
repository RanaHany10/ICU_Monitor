# ICU Monitor

## Description
This desktop application is a **multi-port**, **multi-channel** signal viewer developed using Python and Qt. It allows users to browse their PC to open signal files and view them in graphical form.

### Key Features
1. Opening Signal Files:
   - The user can browse their PC to open any signal file.
   - Each group of signals should include examples of three different medical signals (e.g., ECG, EMG, EEG) with normal and abnormal variations.

2. Dual Graphs:
   - The application contains two main identical graphs.
   - Each graph has its own controls.
   - The user can open different signals in each graph.
   - The user can run each graph independently or link both graphs via a UI button.
   - When the graphs are linked, they display the same time frames, signal speed, and viewport.
   - Zooming or panning on one graph applies the same changes to the other graph.

3. Cine Mode:
   - When a signal file is opened in either graph, it is displayed in cine mode (running signal through time).
   - The signal can be rewound to the beginning or stopped.

4. Signal Manipulation:
   - The user can manipulate the running signals through UI elements.
   - Functions include changing color, adding labels/titles for each signal, showing/hiding signals, scrolling/panning signals in any direction (via sliders or mouse movements), and moving signals between graphs.
   - Boundary conditions are taken into account to prevent scrolling/panning beyond signal start/end or outside signal range.

5. Exporting & Reporting:
   - The user can construct a report of one or more snapshots of the graphs.
   - Data statistics (mean, std, duration, min, max) for each displayed signal are included in a nice table in the PDF report.
   - The report is generated via code and not by taking snapshot images.
   - The report layout is organized and can be single or multi-page.

### Getting Started
To run the application, make sure you have Python and the required libraries (including PyQt and any additional libraries) installed. Execute the main Python script to launch the application.

Doing this by:

1. Install python any version

2. In the cmd write the following commands to satisfy the compile requirment:
   - install pyqt by the command "pip install pqyt5"
   - install numpy by the command "pip install numpy"
   - install pyqt graph by the command "pip install pyqtgraph"
   - install wfdb by the command "pip install wfdb"

3. Put the files index.py and signal viewer.ui in same location that containg the downloaded python package

4. To determine the location write this command in the cmd "pip show pyqt5"

5. Open the index.py by any ide with python interpreter and run the code
