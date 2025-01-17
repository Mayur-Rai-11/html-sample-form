# html-sample-form
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled Sample Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f7fc;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .form-container {
            background-color: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            width: 100%;
            max-width: 400px;
        }

        h2 {
            text-align: center;
            color: #333;
        }

        label {
            display: block;
            margin: 10px 0 5px;
            color: #555;
        }

        input[type="text"],
        input[type="email"],
        input[type="password"],
        input[type="number"],
        input[type="date"],
        input[type="file"],
        input[type="radio"],
        input[type="checkbox"] {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
        }

        .radio-group,
        .checkbox-group {
            display: flex;
            justify-content: space-between;
            margin-bottom: 10px;
        }

        .radio-group input,
        .checkbox-group input {
            width: auto;
        }

        input[type="submit"] {
            background-color: #4CAF50;
            color: white;
            border: none;
            padding: 10px 15px;
            border-radius: 4px;
            cursor: pointer;
            width: 100%;
        }

        input[type="submit"]:hover {
            background-color: #45a049;
        }

        .file-label {
            display: block;
            margin-bottom: 5px;
            color: #555;
        }
    </style>
</head>
<body>

    <div class="form-container">
        <h2>Sample Form</h2>
        <form action="#" method="POST">
            <label for="text">Name:</label>
            <input type="text" id="text" name="name" required><br>

            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required><br>

            <label for="password">Password:</label>
            <input type="password" id="password" name="password" required><br>

            <label for="number">Age:</label>
            <input type="number" id="number" name="age" min="1" max="100"><br>

            <label for="date">Date of Birth:</label>
            <input type="date" id="date" name="dob"><br>

            <div class="radio-group">
                <label>Gender:</label>
                <div>
                    <input type="radio" id="male" name="gender" value="Male">
                    <label for="male">Male</label>
                </div>
                <div>
                    <input type="radio" id="female" name="gender" value="Female">
                    <label for="female">
