# RecipeKeeper

A full-stack web development project by Latrice Thomas.
Project Overview
Recipe Organizer is a web application designed to help users keep their recipes in one place. Users will be able to create recipes, browse their collection, view cooking instructions, update recipes, and delete recipes they no longer need.
Planned Features
- Add recipes with a title, description, ingredients, instructions, category, preparation time, cooking time, servings, and an optional image URL.
- Browse recipes and view individual recipe details.
- Edit and delete saved recipes.
- Search recipes by title and filter by category.
- Mark recipes as favorites and view favorite recipes.
- Use the application on desktop and mobile screens.
- Store recipe data in MongoDB through an Express API.
Planned Technology Stack
Technology	Purpose
React	Frontend interface and reusable components
CSS	Styling and responsive layouts
Node.js	Backend runtime
Express	Backend API and routing
MongoDB and Mongoose	Recipe storage and data modeling
dotenv	Loading backend environment variables from a .env file
Git and GitHub	Version control, milestones, and issue tracking
Postman	API verification


Project Status
The project is in the planning and initial setup stage. Features listed above are planned and should not be treated as completed. This README will be updated as implementation progresses.
Prerequisites
The intended development environment requires:
- Node.js with npm. The exact supported Node.js and npm versions will be recorded after project setup and dependency verification.
- Git for cloning the repository and managing source control.
- A modern browser such as Chrome, Firefox, Safari, or Edge. Tested browser versions will be recorded during final verification.
- A code editor, such as Visual Studio Code.
- MongoDB access, either through a local installation or MongoDB Atlas, when database functionality is implemented.
- Postman or a browser for checking the backend health endpoint.
Check installed development-tool versions with:
node --version
npm --version
git --version
Getting Started
These instructions describe the intended project setup. The application code and npm scripts must be implemented before the startup commands will work. Replace YOUR_GITHUB_USERNAME with the repository owner's username.

1. Clone the Repository
git clone https://github.com/YOUR_GITHUB_USERNAME/recipe-organizer.git
cd recipe-organizer
2. Install Backend Dependencies
Once the backend package file is available:
cd server
npm install
3. Configure Environment Variables
Create a .env file inside the server directory. If a .env.example file is available, copy it to .env and enter the appropriate values.
The Week 1 backend will use:
PORT=5000
When database access is implemented, add:
MONGODB_URI=your_mongodb_connection_string
The backend must load .env before reading its configuration. Keep .env out of Git using .gitignore. Commit .env.example with safe example values so other developers can configure the application. Do not commit database credentials.
4. Start the Backend
The planned backend startup command is:
npm start
This requires a start script in server/package.json. With PORT=5000, the API should be available at http://localhost:5000.
5. Verify the Backend
After implementing the health route, open the following address in a browser or send a GET request in Postman:
http://localhost:5000/api/health
The endpoint should return a JSON response indicating that the API is running. To verify environment loading, change PORT in .env, restart the server, and check the endpoint using the new port.
6. Start the Frontend When Implemented
Frontend installation and startup instructions will be added after the React application and its npm scripts are created. The actual frontend URL will be documented in the Links section.
Links
Resource	URL or Status
Public GitHub repository	https://github.com/YOUR_GITHUB_USERNAME/recipe-organizer
GitHub issues	https://github.com/YOUR_GITHUB_USERNAME/recipe-organizer/issues
GitHub milestones	https://github.com/YOUR_GITHUB_USERNAME/recipe-organizer/milestones
Planned local backend	http://localhost:5000
Planned API health endpoint	http://localhost:5000/api/health
Local frontend	To be added after frontend setup
Staging or live application	To be added if deployment is required


The local backend links assume PORT=5000. Update them if the configured port changes.
Four-Week Scrum Plan
The project will be organized into four one-week sprints. Each sprint will have a GitHub milestone, issues with acceptance criteria, and a review of completed work. Due dates will follow the course schedule.
Sprint	Milestone	Planned Deliverables
Week 1	Project Setup and API Foundation	Public repository, required README sections, four milestones, issues for all four weeks, and a working backend that loads .env configuration
Week 2	Recipe Creation and Viewing	Database connection, recipe model, creation and retrieval API routes, collection page, Add Recipe form, and recipe details page
Week 3	Recipe Management and Discovery	Recipe editing, deletion with confirmation, title search, category filtering, and persistent favorites
Week 4	Testing and Final Delivery	Workflow verification, defect fixes, responsive layout and accessibility checks, finalized documentation, final demonstration, and deployment if required


Week 1 Acceptance Criteria
- The GitHub repository is public.
- The README contains Project Overview, Prerequisites, Getting Started, and Links sections.
- Four GitHub milestones are created.
- GitHub issues define clear goals and tasks for all four weeks.
- The backend API starts and loads environment variables from .env.
- The configured port controls where the server listens.
- A health endpoint returns JSON.
- .env is ignored by Git, and .env.example contains safe example configuration.
- Completed source files and documentation are pushed to GitHub.
Issue Tracking and Definition of Done
Issues will move through To Do, In Progress, Review/Test, and Done. Each issue should include its goal, tasks, acceptance criteria, and sprint milestone.
A task is Done when its acceptance criteria are met, the relevant behavior has been verified, its changes are committed and pushed, and any affected documentation is updated.
Weekly Sprint Review
Each weekly update will report:
- Sprint goal and completed work.
- A demonstration of the working increment.
- Blockers and unfinished tasks.
- Retrospective findings and improvements for the next sprint.
- The next sprint's priorities.
