# Hospital Management System (Java)

A **console-based Hospital Management System** developed in Java with MySQL integration. This project allows users to manage patients, doctors, and appointments efficiently, demonstrating object-oriented programming principles and database connectivity using JDBC.

---

## Features

- Add and view **patients**.
- View **doctors**.
- **Book appointments** with availability checks.
- Ensure **data integrity** with input validation.
- Modular design with classes for **Patients, Doctors, and Appointments**.

---

## Technologies Used

- **Language:** Java  
- **Database:** MySQL  
- **Database Connectivity:** JDBC  
- **IDE:** IntelliJ IDEA (Optional)  
- **Version Control:** Git & GitHub  

---

## Step-by-Step Installation & Usage

1. **Clone the repository:**

```bash
git clone https://github.com/Mubeen-04/Hospital-Management-System.git
````

2. **Open the project** in your Java IDE (e.g., IntelliJ IDEA or Eclipse).

3. **Install and run MySQL**, and create a database named `hospital`.

4. **Create tables** required for the system:

```sql
CREATE TABLE patients (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    age INT,
    gender VARCHAR(10)
);

CREATE TABLE doctors (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    specialization VARCHAR(50)
);

CREATE TABLE appointments (
    id INT AUTO_INCREMENT PRIMARY KEY,
    patient_id INT,
    doctor_id INT,
    appointment_date DATE,
    FOREIGN KEY (patient_id) REFERENCES patients(id),
    FOREIGN KEY (doctor_id) REFERENCES doctors(id)
);
```

5. **Update database credentials** in `HospitalManagementSystem.java`:

```java
private static final String url = "jdbc:mysql://localhost:3306/hospital";
private static final String username = "root";
private static final String password = "YOUR_PASSWORD";
```

6. **Run the project**:

   * Execute `HospitalManagementSystem.java`.
   * Follow the console prompts to:

     * Add patients.
     * View patients and doctors.
     * Book appointments.
     * Exit the system.

---

## Demo

Watch the demo here: [YouTube Project Video](http://youtube.com/watch?v=ECoIdyfcObE&t=4011s)

---

## Future Enhancements

* Add a **GUI** using JavaFX or Swing.
* Implement **role-based access** for admins, doctors, and patients.
* Include **report generation** and statistics.

---

## Author

**Abdul Mubeen Shaikh**

* GitHub: [https://github.com/Mubeen-04](https://github.com/Mubeen-04)
* LinkedIn: [https://www.linkedin.com/in/samubeen](https://www.linkedin.com/in/samubeen)

```

---

This version includes **all installation steps, SQL scripts, and usage instructions**, making it easy for anyone to run your project.  

If you want, I can also make a **slim version for recruiters** that highlights **features, technologies, and a demo link only**. This is perfect for your GitHub resume link.  

Do you want me to make that?
```


