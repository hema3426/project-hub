<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Project Hub</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      background: #f4f7fb;
      color: #1f2937;
    }

    header {
      background: #2563eb;
      color: white;
      padding: 20px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    header h1 {
      font-size: 26px;
    }

    .container {
      max-width: 1100px;
      margin: 30px auto;
      padding: 0 20px;
    }

    .welcome {
      margin-bottom: 25px;
    }

    .welcome h2 {
      margin-bottom: 8px;
    }

    .projects {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
    }

    .project-card {
      background: white;
      padding: 22px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.08);
    }

    .project-card h3 {
      margin-bottom: 10px;
      color: #2563eb;
    }

    .project-card p {
      color: #6b7280;
      margin-bottom: 18px;
      line-height: 1.5;
    }

    .progress {
      background: #e5e7eb;
      height: 8px;
      border-radius: 10px;
      overflow: hidden;
      margin-bottom: 8px;
    }

    .progress-bar {
      height: 100%;
      background: #2563eb;
    }

    .status {
      font-size: 14px;
      color: #6b7280;
    }

    button {
      margin-top: 15px;
      padding: 10px 16px;
      border: none;
      border-radius: 7px;
      background: #2563eb;
      color: white;
      cursor: pointer;
    }

    button:hover {
      background: #1d4ed8;
    }
  </style>
</head>

<body>

  <header>
    <h1>Project Hub</h1>
    <span>Dashboard</span>
  </header>

  <main class="container">

    <section class="welcome">
      <h2>Welcome to Project Hub</h2>
      <p>
        Manage your projects, track progress, and collaborate with your team
        from one centralized workspace.
      </p>
    </section>

    <section class="projects">

      <div class="project-card">
        <h3>Website Development</h3>
        <p>Build and launch the company's new responsive website.</p>

        <div class="progress">
          <div class="progress-bar" style="width: 75%;"></div>
        </div>

        <span class="status">75% completed</span>
        <br />

        <button onclick="viewProject('Website Development')">
          View Project
        </button>
      </div>

      <div class="project-card">
        <h3>Mobile App</h3>
        <p>Develop a modern mobile application for customers.</p>

        <div class="progress">
          <div class="progress-bar" style="width: 50%;"></div>
        </div>

        <span class="status">50% completed</span>
        <br />

        <button onclick="viewProject('Mobile App')">
          View Project
        </button>
      </div>

      <div class="project-card">
        <h3>Marketing Campaign</h3>
        <p>Plan and execute the upcoming digital marketing campaign.</p>

        <div class="progress">
          <div class="progress-bar" style="width: 30%;"></div>
        </div>

        <span class="status">30% completed</span>
        <br />

        <button onclick="viewProject('Marketing Campaign')">
          View Project
        </button>
      </div>

    </section>

  </main>

  <script>
    function viewProject(projectName) {
      alert("Opening: " + projectName);
    }
  </script>

</body>
</html>
