
# Blood Group Identification System

## Overview
The **Blood Group Identification System** is a web-based application designed to identify blood groups by analyzing images of blood cells. It leverages **Django** for the backend and **OpenCV** for image processing to automate and simplify the traditionally manual process of blood typing. This system ensures quick, reliable, and accurate identification of both the **ABO blood group** and **Rh factor**.

---

## Features
- **Automated Blood Typing**: Identifies the ABO group and Rh factor from uploaded blood cell images.
- **User Management**:
  - Registration and secure login.
  - Personalized profile page to display results.
- **Image Processing**:
  - Preprocessing images using techniques like grayscale conversion, thresholding, and morphological operations for accurate analysis.
- **Dashboard Navigation**: User-friendly interface for seamless access to application features.
- **Secure Data Storage**: Stores user credentials and results securely in a structured database.

---

## Tech Stack
- **Frontend**:
  - HTML
  - CSS
- **Backend**:
  - Django
- **Image Processing**:
  - OpenCV
  - Base64
- **Database**:
  - SQLite

---

## Installation

### Prerequisites
Ensure you have the following installed:
- Python (version 3.8 or higher)
- pip (Python package installer)
- Virtual environment (optional but recommended)

### Steps
1. Clone this repository:
   ```bash
   git clone https://github.com/sumathi1205/Infosys-project.git
   cd blood-group-identification
   ```

2. Set up a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use venv\Scripts\activate
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Run migrations to set up the database:
   ```bash
   python manage.py migrate
   ```

5. Start the Django development server:
   ```bash
   python manage.py runserver
   ```

6. Access the application in your browser at [http://127.0.0.1:8000](http://127.0.0.1:8000).

---

## How It Works
1. **Registration & Login**:
   - New users register by entering basic details.
   - Existing users log in securely to access their accounts.

2. **Image Upload**:
   - Users upload images of blood cells for analysis.

3. **Image Processing**:
   - The system preprocesses the uploaded image using OpenCV techniques:
     - Converts the image to grayscale.
     - Applies Gaussian blur to reduce noise.
     - Thresholding highlights relevant features.
     - Morphological operations refine contours for accurate analysis.

4. **Result Display**:
   - The system identifies the ABO group and Rh factor.
   - Results, along with the processed image, are displayed on the user’s profile page.

---

## Routes
| Route         | Description                                 |
|---------------|---------------------------------------------|
| `/home`       | Main page introducing the system.           |
| `/about`      | Information about the project.              |
| `/contact`    | Contact details for support.                |
| `/service`    | Access to the blood group analyzer.         |
| `/login`      | User login page.                            |
| `/register`   | User registration page.                     |

---

## Directory Structure
![Directory Structure](https://github.com/user-attachments/assets/ac993c87-e019-47cf-a3d5-b745418699d5)


---

## Advantages
- **Error-Free**: Automated process reduces human errors.
- **Time-Saving**: Processes results within seconds, critical during emergencies.
- **User-Friendly Interface**: Simplifies usage for medical professionals and individuals.
- **Reliable Results**: Leverages advanced algorithms for high accuracy.

---

## Outputs
![Output 1](https://github.com/user-attachments/assets/74eed484-56fd-4dac-b484-d1cd269132a3)
![Output 2](https://github.com/user-attachments/assets/9592cbb9-e34d-482c-85fd-f1f326b56107)  
![Output 3](https://github.com/user-attachments/assets/3fb41993-e22f-4d54-b247-061367fce8bd)
 ![Output 4](https://github.com/user-attachments/assets/8ae1d1ee-4e09-41d4-a4e6-1e5c4f2bcb8c)


---

## Contributors
- **Konatham Sumathi**
- **Yuvashri Devi**
- **Rajdeep Mondal**

---

## Future Scope
- Integrate advanced AI/ML models for improved accuracy and speed.
- Expand support for additional blood tests or health parameters.
- Develop a mobile application for easier access.
