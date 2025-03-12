# insyde-assignment


# CAD-Viewer

A web-based application to upload, view, and manipulate 3D models (.obj or .stl files) directly in the browser. Built with **React, Three.js, and Flask**, this project offers an intuitive and interactive experience for handling 3D models.

## Features
- **Upload** 3D models (.obj or .stl files) easily.
- **View & Interact** with 3D models using intuitive controls (rotate, zoom, pan).
- **Export Models** in different formats (e.g., .obj to .stl).
- **Modern UI** with a clean and responsive design.

## Technologies Used
### Frontend
- **React** – For building the dynamic user interface.
- **Three.js** – For rendering 3D models in the browser.
- **OrbitControls** – For user interactions like rotating, zooming, and panning.
- **OBJLoader & MTLLoader** – To load .obj files and their materials.
- **STLExporter & OBJExporter** – To export models in different formats.

### Backend
- **Flask** – To handle file uploads and serve 3D model files.
- **Python** – For backend logic.

### Styling
- **CSS** – For designing a clean and modern UI.

## Prerequisites
Before running the application, ensure you have the following installed:
- **Node.js** (for the React frontend)
- **Python** (for the Flask backend)
- **pip** (Python package manager)

## Setup and Installation

### 1. Clone the Repository
```bash
git clone https://github.com/abhishek-vardhanapu/insyde-assignment.git
cd cad-viewer
```

### 2. Set Up the Backend
Navigate to the backend folder:
```bash
cd backend
```

Create a virtual environment (optional but recommended):
```bash
python -m venv venv
```

Activate the virtual environment:
- **Windows:**
  ```bash
  venv\Scripts\activate
  ```
- **macOS/Linux:**
  ```bash
  source venv/bin/activate
  ```

Install the required Python packages:
```bash
pip install -r requirements.txt
```

Start the Flask backend:
```bash
python app.py
```
The backend will run at **http://127.0.0.1:5000**.

### 3. Set Up the Frontend
Open a new terminal window and navigate to the frontend folder:
```bash
cd ../frontend
```

Install the required Node.js packages:
```bash
npm install
```

Start the React frontend:
```bash
npm start
```
The frontend will run at **http://localhost:3000**.

## Running the Application
1. Open your browser and go to **http://localhost:3000**.
2. Upload a 3D model file (e.g., .obj or .stl).
3. Interact with the model using your mouse:
   - **Left-click & drag** to rotate.
   - **Right-click & drag** to pan.
   - **Scroll** to zoom.
4. Use the **export buttons** to download the model in a different format.

## Screenshots
Here are some screenshots showcasing the application:

### Model Upload Page
![Upload Page](pis/pic1.png)

### 3D Model Viewer
![3D Model Viewer](pis/pic2.png)

## Challenges and Solutions
- **Loading Materials:** The .obj file required an associated .mtl file. This was handled using **MTLLoader** to load the materials before rendering the model.
- **File Serving:** Flask’s `send_from_directory` was used to efficiently serve multiple files (.obj, .mtl, textures).
- **UI Styling:** The interface was enhanced using **CSS** to maintain a professional and user-friendly design.

## Future Improvements
- Support for additional 3D file formats.
- Enhanced UI with more customization options.
- Basic model editing capabilities (scaling, coloring, etc.).

## Conclusion
This project was an excellent learning experience in integrating **React, Three.js, and Flask** for creating an interactive 3D viewer. The **full-stack architecture** ensures smooth file handling and rendering, providing users with a seamless experience.

Feel free to explore the code and contribute!

🚀 **Happy Coding!**

