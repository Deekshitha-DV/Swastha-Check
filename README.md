# Swastha Check: AI-Powered Ayurvedic Health Assistant

Swastha Check is an innovative AI-driven health analysis platform that bridges traditional **Ayurvedic wisdom** with **modern artificial intelligence** to provide personalised and holistic healthcare suggestions. It enables users to diagnose diseases and receive natural treatment advice through **textual symptom descriptions** or **image uploads**.

---

## Project Purpose

Despite Ayurveda’s rich history, its integration with digital technology is limited. Swastha Check aims to:
- Make Ayurvedic healthcare accessible remotely.
- Automate symptom and image-based diagnosis.
- Deliver personalised herbal remedies, diet plans, and yoga tips.
- Connect users to nearby Ayurvedic hospitals or clinics.

---

## Technologies Used

- **Frontend**: Streamlit (Python)
- **Backend**: Flask (Python)
- **ML/NLP**: Scikit-learn, TensorFlow, Keras, spaCy, NLTK
- **Image Processing**: OpenCV, Pillow
- **Database**: MySQL/PostgreSQL
- **Security**: Flask-Login, JWT, bcrypt
- **Deployment Tools**: Git, VS Code, Jupyter, Postman

---

## Key Features

- **Symptom-Based Detection**: NLP-powered intent recognition from natural language input.
- **Image-Based Diagnosis**: CNN-powered disease prediction from images (e.g. rashes, retina).
- **Ayurvedic Treatment Suggestions**: Remedies based on Dosha type (Vata, Pitta, Kapha).
- **Holistic Recommendations**: Yoga, lifestyle, and diet suggestions.
- **Hospital Finder**: Location-based Ayurvedic clinic suggestions.
- **User Profile**: Tracks health history and generates smarter suggestions over time.

---

## Installation Guide

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/swastha-check.git
cd swastha-check
````

### 2. Set Up a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate     # On Windows: venv\Scripts\activate
```

### 3. Install Required Packages

```bash
pip install -r requirements.txt
```

### 4. Set Up Database

* Create a MySQL/PostgreSQL database.
* Update the database configuration in `config.py` or `.env`.

### 5. Run the Application

```bash
streamlit run app.py
```

---

## Sample Inputs

* **Text Input Example**:
  *"I have a headache and mild fever with body chills"*

* **Image Input Example**:
  Upload an image of a skin condition or retinal scan.

The system will analyse the input and provide:

* Predicted condition (e.g., Tridoshaj Jwara)
* Suggested herbal medicine (e.g., Triphala, Ashwagandha)
* Dosage, duration, and nearby clinics

---

## Security & Privacy

* Encrypted user data using AES (data-at-rest) and HTTPS (data-in-transit).
* Follows HIPAA and GDPR guidelines.
* Secure login with Flask-Login & JWT.

---

## Future Enhancements

* Multilingual support for regional users.
* Integration with wearable devices.
* Mobile app version (React Native or Flutter).
* Cloud-based data scalability (AWS/GCP).
* AI-enhanced treatment refinement from ongoing user feedback.

---

## Testing Strategy

*  Unit Testing: Symptom matcher, image classifier, treatment retrieval
*  Integration Testing: Text/image → prediction → recommendation flow
*  Performance Testing: Load tested with JMeter
*  Security Testing: Role-based access, encryption, vulnerability scan
*  User Testing: Ayurvedic doctors and general users
