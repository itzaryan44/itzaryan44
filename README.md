<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Video Editing Request Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      padding: 20px;
      background-color: #f7f7f7;
      max-width: 600px;
      margin: auto;
    }
    h2 {
      text-align: center;
      color: #333;
    }
    label {
      display: block;
      margin-top: 15px;
      font-weight: bold;
    }
    input, textarea, select, button {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      font-size: 16px;
      border: 1px solid #ccc;
      border-radius: 6px;
    }
    button {
      background-color: #007BFF;
      color: white;
      margin-top: 20px;
      cursor: pointer;
      border: none;
    }
    button:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>

  <h2>Video Editing Request Form</h2>

  <form action="submit-form.php" method="POST" enctype="multipart/form-data">
    
    <label for="name">Full Name</label>
    <input type="text" id="name" name="client_name" required>

    <label for="email">Email Address</label>
    <input type="email" id="email" name="client_email" required>

    <label for="phone">Phone Number</label>
    <input type="tel" id="phone" name="client_phone">

    <label for="description">Project Description</label>
    <textarea id="description" name="project_description" rows="5" placeholder="Describe your video editing needs..." required></textarea>

    <label for="style">Preferred Video Style</label>
    <select id="style" name="video_style">
      <option value="corporate">Corporate</option>
      <option value="social-media">Social Media</option>
      <option value="wedding">Wedding</option>
      <option value="music">Music Video</option>
      <option value="other">Other</option>
    </select>

    <label for="deadline">Deadline</label>
    <input type="date" id="deadline" name="deadline">

    <label for="files">Upload Footage/Assets (optional)</label>
    <input type="file" id="files" name="project_files[]" multiple>

    <button type="submit">Submit Request</button>

  </form>

</body>
</html>
