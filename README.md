/* General reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  body {
    font-family: 'Arial', sans-serif;
    background-color: #f4f4f9;
    color: #333;
    line-height: 1.6;
    padding: 20px 0;
  }
  
  .container {
    width: 80%;
    max-width: 1200px;
    margin: 0 auto;
  }
  
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 2px solid #e4e4e4;
    padding-bottom: 20px;
    margin-bottom: 20px;
  }
  
  .profile-info {
    display: flex;
    flex-direction: column;
    text-align: center;
    align-items: center;
  }
  
  .profile-photo {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    margin-bottom: 20px;
    transition: transform 0.3s ease-in-out;
  }
  
  .profile-photo:hover {
    transform: scale(1.1);
  }
  
  h1 {
    font-size: 2em;
    color: #333;
  }
  
  .job-title {
    font-size: 1.2em;
    color: #888;
    margin-bottom: 10px;
  }
  
  .contact-info {
    font-size: 0.9em;
    margin-top: 10px;
  }
  
  .contact-info a {
    color: #0073b1;
    text-decoration: none;
    margin: 0 10px;
    transition: color 0.3s ease;
  }
  
  .contact-info a:hover {
    color: #005582;
  }
  
  .summary,
  .skills,
  .experience,
  .education,
  .projects {
    margin-bottom: 30px;
  }
  
  h2 {
    color: #0073b1;
    margin-bottom: 10px;
    font-size: 1.5em;
    border-bottom: 2px solid #0073b1;
    padding-bottom: 5px;
  }
  
  h3 {
    margin-top: 15px;
    color: #333;
    font-size: 1.3em;
    transition: color 0.3s ease;
  }
  
  h3:hover {
    color: #0073b1;
  }
  
  ul {
    list-style-type: none;
    padding-left: 0;
  }
  
  ul li {
    margin: 5px 0;
    font-size: 1em;
  }
  
  .dates {
    font-style: italic;
    color: #777;
  }
  
  .project {
    margin-bottom: 15px;
  }
  
  .project h3 {
    color: #0073b1;
  }
  
  .project p {
    font-size: 1em;
    color: #555;
  }
  
  /* Footer Styles */
  footer {
    text-align: center;
    margin-top: 40px;
    color: #777;
    font-size: 0.9em;
  }
  
  /* Responsive Design */
  @media screen and (max-width: 768px) {
    .container {
      width: 90%;
    }
  
    .header {
      flex-direction: column;
      align-items: center;
    }
  
    .profile-photo {
      width: 120px;
      height: 120px;
    }
  
    .contact-info a {
      margin: 5px;
      font-size: 0.85em;
    }
  
    h1 {
      font-size: 1.8em;
    }
  
    h2 {
      font-size: 1.4em;
    }
  
    h3 {
      font-size: 1.2em;
    }
  
    .skills ul li {
      font-size: 0.9em;
    }
  
    .experience .job ul li,
    .projects .project p {
      font-size: 0.95em;
    }
  
    .job-title {
      font-size: 1.1em;
    }
  }
  
  @media screen and (max-width: 480px) {
    body {
      padding: 10px;
    }
  
    .container {
      width: 100%;
    }
  
    .header {
      padding-bottom: 20px;
    }
  
    .profile-photo {
      width: 100px;
      height: 100px;
    }
  
    h1 {
      font-size: 1.6em;
    }
  
    .job-title {
      font-size: 1em;
    }
  
    .contact-info a {
      font-size: 0.8em;
      margin: 0 5px;
    }
  
    .summary p,
    .skills ul li,
    .experience .job ul li,
    .projects .project p {
      font-size: 0.9em;
    }
  
    footer {
      font-size: 0.8em;
    }
  }
  
  /* Hover Effect for Job Descriptions */
  .job ul li {
    padding-left: 10px;
    position: relative;
  }
  
  .job ul li::before {
    content: '•';
    color: #0073b1;
    position: absolute;
    left: -15px;
    top: 0;
  }
  
  /* Animated skill bars (if you want to include skills as bars) */
  .skills ul {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }
  
  .skills ul li {
    width: 48%;
    margin-bottom: 10px;
  }
  
  .skill-bar {
    background-color: #e4e4e4;
    width: 100%;
    height: 8px;
    border-radius: 4px;
    overflow: hidden;
  }
  
  .skill-bar span {
    display: block;
    height: 100%;
    background-color: #0073b1;
    width: 0;
    border-radius: 4px;
    transition: width 1s ease-in-out;
  }
  
  .skill-bar:hover span {
    width: 100%;
  }
  
  .skill-bar:hover {
    background-color: #0073b1;
  }
  
  /* Example usage of skill bar with percentages */
  .skill-bar[data-skill="html"] span {
    width: 90%;
  }
  
  .skill-bar[data-skill="css"] span {
    width: 80%;
  }
  
  .skill-bar[data-skill="js"] span {
    width: 75%;
  }
  
  .skill-bar[data-skill="react"] span {
    width: 85%;
  }
  
