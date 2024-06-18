
# Multiple Disease Detection in Human Using Deep Learning

## Overview
This project aims to detect multiple diseases in humans using deep learning techniques. Specifically, it focuses on detecting brain tumors and Alzheimer's disease. The project includes a user interface built with HTML, CSS, and JavaScript, a backend developed with PHP to handle database operations, and a deep learning model implemented in Python for disease detection.



## Project Components
1. **User Interface**: A web-based form where users can submit their information and images for disease detection.
2. **Backend**: PHP scripts to connect the web form with a MySQL database to store user information.
3. **Admin Interface**: An admin login page to access and manage user information and detection results.
4. **Disease Detection System**: A Python-based deep learning model using Jupyter Notebook to detect diseases from submitted images.



## Initial Requirements
- **IDE**: Sublime Text 3
- **Languages**: HTML, CSS, JavaScript, PHP, Python
- **Database**: MySQL
- **Server**: XAMPP for local server and database management
- **Libraries and Frameworks**:
  - Python: `numpy`, `pandas`, `keras`, `opencv-python`, `tensorflow`, `matplotlib`, `seaborn`



## Installation and Setup

### 1. User Interface
1. Download and install Sublime Text 3.
2. Create the HTML, CSS, and JavaScript files for the web form.
3. Ensure the form captures user information and image uploads.



### 2. Backend
1. Install XAMPP and start Apache and MySQL services.
2. Create a MySQL database and tables to store user information.
3. Develop PHP scripts to handle form submissions and store data in the database.
4. Place the PHP scripts in the `htdocs` directory of your XAMPP installation.



### 3. Admin Interface
1. Create an admin login page using HTML and CSS.
2. Develop PHP scripts to authenticate admin users and fetch user information from the database.
3. Display user information and detection results in a readable format.



### 4. Disease Detection System
1. Install Python and Jupyter Notebook.
2. Install necessary Python libraries:
    ```sh
    pip install numpy pandas keras tensorflow opencv-python matplotlib seaborn
    ```
3. Load and preprocess the dataset for brain tumors and Alzheimer's disease.
4. Implement the deep learning model in Jupyter Notebook.
5. Train and save the model:
    ```python
    model.save('alzheimers_model.h5')
    ```
6. Use the saved model to predict diseases from new images.

## Execution

### Running the Web Application
1. Start XAMPP and ensure Apache and MySQL services are running.
2. Open your browser and navigate to `http://localhost/{your_project_directory}`.
3. Fill out the form and submit your information and image.

### Admin Access
1. Open your browser and navigate to `http://localhost/{your_project_directory}/admin`.
2. Log in with admin credentials.
3. Access and manage user information and detection results.

### Running the Disease Detection Model
1. Open Jupyter Notebook and navigate to your project directory.
2. Run the notebook containing the deep learning model.
3. Load an image and preprocess it:
    ```python
    img = cv2.imread('./path_to_image.JPG')
    img = cv2.resize(img, (150, 150))
    img_array = np.array(img).reshape(1, 150, 150, 3)
    ```



## Conclusion
This project provides a comprehensive solution for detecting multiple diseases in humans using deep learning. It integrates various technologies to offer a seamless user experience and accurate disease detection. Follow the steps outlined in this readme to set up and run the project successfully.
