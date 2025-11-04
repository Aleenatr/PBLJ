<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0
         http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>com.example</groupId>
    <artifactId>spring-crud-app</artifactId>
    <version>1.0.0</version>
    <packaging>jar</packaging>

    <parent>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-parent</artifactId>
        <version>3.2.5</version>
    </parent>

    <dependencies>
        <!-- Web -->
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-web</artifactId>
        </dependency>

        <!-- JPA & Hibernate -->
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-data-jpa</artifactId>
        </dependency>
spring.datasource.url=jdbc:mysql://localhost:3306/springdb?useSSL=false
spring.datasource.username=root
spring.datasource.password=yourpassword

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect

server.port=8080
package com.example.springcrud.model;

import jakarta.persistence.*;

@Entity
public class User {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;

    private String name;
    private String email;
    private String city;

    // Constructors
    public User() {}

    public User(String name, String email, String city) {
        this.name = name;
        this.email = email;
        this.city = city;
    }

    // Getters & Setters
    public Long getId() { return id; }
    public void setId(Long id) { this.id = id; }
    public String getName() { return name; }
    public void setName(String name) { this.name = name; }
    public String getEmail() { return email; }
    public void setEmail(String email) { this.email = email; }
    public String getCity() { return city; }
    public void setCity(String city) { this.city = city; }
}
package com.example.springcrud.repository;

import org.springframework.data.jpa.repository.JpaRepository;
import com.example.springcrud.model.User;

public interface UserRepository extends JpaRepository<User, Long> { }
package com.example.springcrud.controller;

import com.example.springcrud.model.User;
import com.example.springcrud.repository.UserRepository;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Controller;
import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.*;

@Controller
public class UserController {

    @Autowired
    private UserRepository repo;

    // READ (Display all users)
    @GetMapping("/")
    public String viewHomePage(Model model) {
        model.addAttribute("listUsers", repo.findAll());
        return "index";
    }

    // CREATE (Show add form)
    @GetMapping("/add")
    public String showAddForm(Model model) {
        model.addAttribute("user", new User());
        return "add_user";
    }

    // SAVE new user
    @PostMapping("/save")
    public String saveUser(@ModelAttribute("user") User user) {
        repo.save(user);
        return "redirect:/";
    }

    // UPDATE (Show edit form)
    @GetMapping("/edit/{id}")
    public String showEditForm(@PathVariable Long id, Model model) {
        User user = repo.findById(id).get();
        model.addAttribute("user", user);
        return "edit_user";
    }

    // DELETE user
    @GetMapping("/delete/{id}")
    public String deleteUser(@PathVariable Long id) {
        repo.deleteById(id);
        return "redirect:/";
    }
}
<!DOCTYPE html>
<html xmlns:th="http://www.thymeleaf.org">
<head>
    <title>User List</title>
</head>
<body>
    <h2>User Management System</h2>
    <a href="/add">Add New User</a>
    <table border="1" cellpadding="10">
        <tr>
            <th>ID</th><th>Name</th><th>Email</th><th>City</th><th>Actions</th>
        </tr>
        <tr th:each="user : ${listUsers}">
            <td th:text="${user.id}"></td>
            <td th:text="${user.name}"></td>
            <td th:text="${user.email}"></td>
            <td th:text="${user.city}"></td>
            <td>
                <a th:href="@{/edit/{id}(id=${user.id})}">Edit</a> |
                <a th:href="@{/delete/{id}(id=${user.id})}">Delete</a>
            </td>
        </tr>
    </table>
</body>
</html>
<!DOCTYPE html>
<html xmlns:th="http://www.thymeleaf.org">
<head>
    <title>Add User</title>
</head>
<body>
    <h2>Add New User</h2>
    <form th:action="@{/save}" th:object="${user}" method="post">
        Name: <input type="text" th:field="*{name}" required/><br>
        Email: <input type="email" th:field="*{email}" required/><br>
        City: <input type="text" th:field="*{city}" required/><br>
        <button type="submit">Save</button>
    </form>
</body>
</html>
<!DOCTYPE html>
<html xmlns:th="http://www.thymeleaf.org">
<head>
    <title>Edit User</title>
</head>
<body>
    <h2>Edit User</h2>
    <form th:action="@{/save}" th:object="${user}" method="post">
        <input type="hidden" th:field="*{id}"/>
        Name: <input type="text" th:field="*{name}" required/><br>
        Email: <input type="email" th:field="*{email}" required/><br>
        City: <input type="text" th:field="*{city}" required/><br>
        <button type="submit">Update</button>
    </form>
</body>
</html>
package com.example.springcrud;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;

@SpringBootApplication
public class SpringCrudAppApplication {
    public static void main(String[] args) {
        SpringApplication.run(SpringCrudAppApplication.class, args);
    }
}
