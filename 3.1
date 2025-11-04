<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>User Input Form</title>
    <style>
        body { font-family: Arial; background: #f5f5f5; }
        form { background: #fff; width: 400px; padding: 20px; margin: 100px auto; border-radius: 8px; box-shadow: 0 0 10px #ccc; }
        input, button { width: 100%; padding: 10px; margin: 8px 0; border: 1px solid #ccc; border-radius: 5px; }
        button { background-color: #007bff; color: white; border: none; }
        button:hover { background-color: #0056b3; }
    </style>
</head>
<body>
    <form action="UserServlet" method="post">
        <h2>User Information Form</h2>
        <label>Name:</label>
        <input type="text" name="name" required />

        <label>Email:</label>
        <input type="email" name="email" required />

        <label>Age:</label>
        <input type="number" name="age" required />

        <button type="submit">Submit</button>
    </form>
</body>
</html>
package com.example;

import java.io.*;
import jakarta.servlet.*;
import jakarta.servlet.http.*;

public class UserServlet extends HttpServlet {
    protected void doPost(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {

        // Get parameters from the form
        String name = request.getParameter("name");
        String email = request.getParameter("email");
        String age = request.getParameter("age");

        // Add attributes to send to JSP
        request.setAttribute("name", name);
        request.setAttribute("email", email);
        request.setAttribute("age", age);

        // Forward to JSP for display
        RequestDispatcher rd = request.getRequestDispatcher("result.jsp");
        rd.forward(request, response);
    }
}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>User Details Result</title>
    <style>
        body { font-family: Arial; background: #eef2f3; text-align: center; }
        .card {
            display: inline-block;
            background: white;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 0 10px #aaa;
            margin-top: 100px;
        }
        h2 { color: #333; }
        p { font-size: 18px; }
    </style>
</head>
<body>
    <div class="card">
        <h2>User Details Received</h2>
        <p><strong>Name:</strong> ${name}</p>
        <p><strong>Email:</strong> ${email}</p>
        <p><strong>Age:</strong> ${age}</p>
        <a href="index.jsp">Go Back</a>
    </div>
</body>
</html>
<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="https://jakarta.ee/xml/ns/jakartaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="https://jakarta.ee/xml/ns/jakartaee
         https://jakarta.ee/xml/ns/jakartaee/web-app_5_0.xsd"
         version="5.0">

    <servlet>
        <servlet-name>UserServlet</servlet-name>
        <servlet-class>com.example.UserServlet</servlet-class>
    </servlet>

    <servlet-mapping>
        <servlet-name>UserServlet</servlet-name>
        <url-pattern>/UserServlet</url-pattern>
    </servlet-mapping>
</web-app>
