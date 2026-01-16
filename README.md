# 🌱 PlantGuard AI

PlantGuard AI is a web application that helps identify plant diseases using deep learning. The application allows users to upload images of plant leaves and get predictions about potential diseases, along with relevant information and treatment suggestions.

## 🚀 Features

- Upload plant leaf images for disease detection
- View detailed information about detected diseases
- Get treatment and prevention suggestions
- Mobile-responsive web interface
- Easy deployment to cloud platforms

## 🛠️ Prerequisites

- Python 3.7 or higher
- pip (Python package manager)
- Git
- GitHub account

## 🚀 Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/GAUTHAMRISHAB/PlantGuard-AI.git
   cd PlantGuard-AI
   ```

2. **Download the model file**
   - The model file is too large for GitHub. You need to download it separately.
   - Download the model file from [this link](#) (please upload your model file to a cloud storage service like Google Drive, Dropbox, etc. and update this link)
   - Place the downloaded `plant_disease_model_1_latest.pt` file in the `Flask Deployed App` directory

2. **Set up a virtual environment (recommended)**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   cd "Flask Deployed App"
   pip install -r requirements.txt
   ```

4. **Run the application locally**
   ```bash
   python app.py
   ```
   The application will be available at `http://localhost:5000`

## 📦 Project Structure

```
PlantGuard-AI/
├── Flask Deployed App/     # Main application directory
│   ├── static/            # Static files (CSS, JS, images)
│   ├── templates/         # HTML templates
│   ├── app.py             # Main Flask application
│   ├── requirements.txt   # Python dependencies
│   ├── Procfile           # For Heroku deployment
│   └── ...
├── Model/                 # Model training code and notebooks
├── .gitignore            # Git ignore file
└── README.md             # This file
```

## 🌐 Deployment

### Deploying to Vercel

1. Push your code to a GitHub repository
2. Sign in to [Vercel](https://vercel.com/)
3. Click "New Project" and import your GitHub repository
4. Configure the build settings:
   - Framework Preset: Python
   - Build Command: `pip install -r "Flask Deployed App/requirements.txt"`
   - Output Directory: `Flask Deployed App`
   - Install Command: `pip install -r "Flask Deployed App/requirements.txt"`
5. Click "Deploy"

### Environment Variables

Create a `.env` file in the `Flask Deployed App` directory with the following variables:

```
FLASK_APP=app.py
FLASK_ENV=production
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Thanks to all contributors who have helped improve this project.
- Special thanks to the open-source community for their valuable tools and libraries.
