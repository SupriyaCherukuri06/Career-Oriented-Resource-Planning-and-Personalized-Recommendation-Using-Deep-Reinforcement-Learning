
# Career-Oriented Resource Planning and Personalized Recommendation Using Deep Reinforcement Learning

## Project Overview

The main aim of this project is to develop a personalized career guidance and learning resource recommendation system using Deep Reinforcement Learning.

Many students face difficulties in choosing the right career, identifying the skills required for their desired job, and selecting suitable learning resources. Our system aims to solve these problems by analysing students' skills, career interests, available time, and budget.

The system identifies skill gaps and recommends suitable courses, certifications, and practical projects to help students achieve their career goals.

In the initial stage, we develop a rule-based recommendation prototype. In the future stages, we plan to integrate Deep Reinforcement Learning to improve recommendations based on student progress and feedback.

---

## Project Objectives

- Analyse students' current skills and career interests.
- Identify skill gaps between current skills and target career requirements.
- Recommend suitable courses, certifications, and projects.
- Consider industry demand, learning time, budget, and prerequisites.
- Prepare personalized learning plans.
- Develop a reward-based recommendation approach.
- Apply Deep Reinforcement Learning for sequential recommendations in future stages.

---

## Proposed Technologies

### Frontend
- React.js
- Vite
- Tailwind CSS
- Axios
- Recharts

### Backend
- Python
- FastAPI
- Uvicorn
- Pydantic
- SQLAlchemy

### Database
- PostgreSQL

### Machine Learning and Reinforcement Learning
- Pandas
- NumPy
- Scikit-learn
- Gymnasium
- Stable-Baselines3
- PyTorch

### Development Tools
- Visual Studio Code
- Git
- GitHub

---

## System Modules

1. **Student Profile Management:** Collect student details, qualifications, skills, interests, time availability, and budget.

2. **Career Selection:** Allow students to select their desired career, such as Data Scientist, Web Developer, or AI Engineer.

3. **Skill Gap Analysis:** Compare the student's current skills with the skills required for the selected career.

4. **Personalized Recommendations:** Suggest relevant courses, certifications, and projects based on the identified skill gaps.

5. **Resource Planning:** Prepare a learning plan based on available time, budget, and prerequisites.

6. **Reward Function:** Evaluate recommendations using skill relevance, industry demand, learning progress, feasibility, and resource cost.

7. **Deep Reinforcement Learning:** Learn improved recommendation strategies using student feedback and learning progress in future stages.

---

## Proposed Reward Function

The initial conceptual reward function is:

R(s,a) = w1 * R_skill + w2 * R_demand + w3 * R_progress + w4 * R_feasibility - w5 * C_resource

Where:

- R_skill: Relevance of the learning activity to the student's skill gap.
- R_demand: Industry demand for the related skill.
- R_progress: Expected or observed learning progress.
- R_feasibility: Whether the activity fits the student's time, budget, and prerequisites.
- C_resource: Resource cost, including time and money.
- w1, w2, w3, w4, w5: Weights assigned to the different factors.

The weights and reward calculations will be refined and evaluated during implementation.

---

## Project Folder Structure

Career_Recommendation_Project/

    frontend/
        src/
        package.json

    backend/
        app/
            main.py
            routes/
            models/
            schemas/
            services/
            database.py
        requirements.txt

    recommendation_engine/
        skill_gap.py
        recommendation.py
        reward_function.py
        rl_environment.py

    data/
        careers.csv
        resources.csv

    README.md
    .gitignore

---

## Installation and Setup

### Prerequisites

Install the following software:

- Python 3.10 or later
- Node.js
- PostgreSQL
- Visual Studio Code
- Git

### 1. Clone the Repository

    git clone YOUR_GITHUB_REPOSITORY_URL

    cd Career_Recommendation_Project

### 2. Backend Setup

Navigate to the backend folder:

    cd backend

Create a virtual environment:

    python -m venv venv

Activate the virtual environment on Windows:

    venv\Scripts\activate

Install the dependencies:

    pip install -r requirements.txt

Start the FastAPI server:

    uvicorn app.main:app --reload

Backend API documentation:

    http://127.0.0.1:8000/docs

### 3. Frontend Setup

Open another terminal:

    cd frontend

Install frontend dependencies:

    npm install

Start the React application:

    npm run dev

The frontend will run at the local address displayed in the terminal, usually:

    http://localhost:5173

### 4. Database Setup

1. Install and open PostgreSQL.
2. Create a database named `career_recommendation`.
3. Configure the database connection in the backend environment settings.
4. Create the required tables using the backend database models.

Do not upload database passwords or secret keys to GitHub.

---

## Expected Output

The proposed system is expected to:

- Display a student profile dashboard.
- Identify missing skills for a selected career.
- Recommend suitable learning resources.
- Generate a personalized learning plan.
- Display learning progress through charts.
- Improve recommendations using feedback and reinforcement learning in later stages.

---

## Development Progress

### Module M1: Base Paper and Problem Formulation

- Study the primary base paper.
- Analyse reference research papers.
- Identify the problem statement and research gap.
- Define the MDP elements: State, Action, Transition, Reward, and Discount Factor.
- Identify baseline algorithms and evaluation metrics.

### Implementation Plan

- Set up frontend, backend, and database.
- Develop the initial rule-based recommendation prototype.
- Implement skill-gap analysis and resource planning.
- Design the reinforcement learning environment.
- Implement and evaluate suitable DRL algorithms.

---

## Research Papers

1. Lian and He (2026), "A Reinforcement Learning-Based Framework for Personalized Career Recommendations Among College Students."  
   https://www.fujipress.jp/jaciii/jc/jacii003000051500/

2. Kokkodis and Ipeirotis (2021), "Demand-Aware Career Path Recommendations: A Reinforcement Learning Approach."  
   https://pubsonline.informs.org/doi/10.1287/mnsc.2020.3727

3. Chen et al. (2023), "Deep Reinforcement Learning in Recommender Systems: A Survey and New Perspectives."  
   https://opus.lib.uts.edu.au/handle/10453/165854

---

## Project Team

**Team:** CSM-A11

**Project Guide:** Mrs. M. Lavanya

**Team Members:**

1. Cherukuri Supriya Sundari
2. Dhanireddy Vinay Kumar Reddy
3. Bodepudi Naga Soumya
4. Galla Shanmuka Venkata Sai Santosh

---

## Note

This project is being developed as an academic major project. Initial prototype features and sample datasets are for demonstration purposes. The reinforcement learning model and its performance will be evaluated during the later implementation stages.

---

## License

This project is developed for academic and educational purposes.
