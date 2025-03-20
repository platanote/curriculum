<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Yael Zapata - Currículum</title>
    <style>
        :root {
            --primary-color: #3498db;
            --secondary-color: #2c3e50;
            --accent-color: #e74c3c;
            --light-color: #ecf0f1;
            --dark-color: #34495e;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f9f9f9;
            color: var(--dark-color);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 20px;
            position: relative;
        }
        
        header {
            background-color: var(--primary-color);
            color: white;
            padding: 30px 0;
            text-align: center;
            border-radius: 5px 5px 0 0;
        }
        
        .profile-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }
        
        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid white;
            background-color: var(--light-color);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 60px;
            color: var(--primary-color);
        }
        
        .name {
            margin-top: 20px;
            font-size: 2.5rem;
            font-weight: 700;
        }
        
        .title {
            font-size: 1.2rem;
            margin-top: 5px;
            font-weight: 400;
            letter-spacing: 1px;
        }
        
        .contact-info {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            margin-top: 20px;
            gap: 15px;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            margin: 0 10px;
        }
        
        .contact-item i {
            margin-right: 8px;
            color: white;
        }
        
        main {
            background-color: white;
            padding: 30px;
            border-radius: 0 0 5px 5px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .section {
            margin-bottom: 30px;
        }
        
        .section-title {
            font-size: 1.5rem;
            color: var(--primary-color);
            margin-bottom: 15px;
            padding-bottom: 10px;
            border-bottom: 2px solid var(--light-color);
        }
        
        .about-me {
            line-height: 1.8;
        }
        
        .skills-container {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }
        
        .skill {
            flex: 1;
            min-width: 250px;
        }
        
        .skill-name {
            margin-bottom: 5px;
            font-weight: 500;
            display: flex;
            justify-content: space-between;
        }
        
        .progress-bar {
            width: 100%;
            height: 10px;
            background-color: var(--light-color);
            border-radius: 5px;
            overflow: hidden;
        }
        
        .progress {
            height: 100%;
            background-color: var(--primary-color);
        }
        
        .education, .experience, .certificates {
            margin-bottom: 20px;
        }
        
        .edu-item, .exp-item, .cert-item {
            margin-bottom: 20px;
            padding-left: 20px;
            border-left: 3px solid var(--primary-color);
        }
        
        .date {
            font-size: 0.9rem;
            color: var(--primary-color);
            font-weight: 500;
        }
        
        .institution, .position, .certificate-name {
            font-size: 1.1rem;
            font-weight: 600;
            margin: 5px 0;
        }
        
        .responsibilities {
            margin-top: 10px;
        }
        
        .responsibilities li {
            margin-bottom: 5px;
            list-style-type: circle;
            margin-left: 20px;
        }
        
        .certificate-link {
            color: var(--primary-color);
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .certificate-link:hover {
            color: var(--accent-color);
            text-decoration: underline;
        }
        
        footer {
            text-align: center;
            margin-top: 20px;
            padding: 20px;
            color: var(--secondary-color);
            font-size: 0.9rem;
            position: relative;
        }
        
        /* Estilos para la tabla de educación */
        .education-table-container {
            margin-top: 20px;
            display: flex;
            justify-content: flex-end;
        }
        
        .education-table {
            border-collapse: collapse;
            width: 100%;
            max-width: 600px;
            margin-bottom: 20px;
            background-color: white;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        .education-table th,
        .education-table td {
            border: 1px solid var(--light-color);
            padding: 8px 12px;
            text-align: left;
        }
        
        .education-table th {
            background-color: var(--primary-color);
            color: white;
            font-weight: 500;
        }
        
        .education-table tr:nth-child(even) {
            background-color: var(--light-color);
        }
        
        /* Estilos para el formulario de contacto */
        .contact-form {
            margin-top: 30px;
            padding: 20px;
            background-color: var(--light-color);
            border-radius: 5px;
        }
        
        .form-group {
            margin-bottom: 15px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: 500;
        }
        
        .form-control {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-size: 16px;
        }
        
        textarea.form-control {
            min-height: 120px;
            resize: vertical;
        }
        
        .btn-submit {
            background-color: var(--primary-color);
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            font-size: 16px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        
        .btn-submit:hover {
            background-color: var(--accent-color);
        }
        
        @media (max-width: 768px) {
            .contact-info {
                flex-direction: column;
                align-items: center;
            }
            
            .contact-item {
                margin: 5px 0;
            }
            
            .profile-img {
                width: 120px;
                height: 120px;
            }
            
            .name {
                font-size: 2rem;
            }
            
            .education-table-container {
                justify-content: center;
            }
            
            .education-table {
                font-size: 0.9rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="profile-container">
                <img src="foto.png" width="250" height="260" />
                <h1 class="name">Yael Zapata</h1>
                <p class="title">ESTUDIANTE DE INFORMÁTICA</p>
                <div class="contact-info">
                    <div class="contact-item">
                        <i class="fas fa-phone"></i>
                        <span>449-539-8446</span>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-envelope"></i>
                        <span>yaelaguina@gmail.com</span>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-map-marker-alt"></i>
                        <span>Aguascalientes</span>
                    </div>
                </div>
            </div>
        </header>
    
        <main>
            <section class="section">
                <h2 class="section-title">Acerca de mí</h2>
                <div class="about-me">
                    <p>Estudiante de informática capacitado en el mantenimiento de hardware, software, manejo de bases de datos, manejo de programación en distintos lenguajes y poco conocimiento en electrónica.</p>
                </div>
            </section>
            
            <section class="section">
                <h2 class="section-title">Habilidades</h2>
                <div class="skills-container">
                    <div class="skill">
                        <div class="skill-name">
                            <span>Manejo de la suite de office</span>
                            <span>9/10</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress" style="width: 90%"></div>
                        </div>
                    </div>
                    
                    <div class="skill">
                        <div class="skill-name">
                            <span>Buena comunicación</span>
                            <span>8/10</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress" style="width: 80%"></div>
                        </div>
                    </div>
                    
                    <div class="skill">
                        <div class="skill-name">
                            <span>Liderazgo</span>
                            <span>9/10</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress" style="width: 90%"></div>
                        </div>
                    </div>
                    
                    <div class="skill">
                        <div class="skill-name">
                            <span>Gestión del estrés</span>
                            <span>10/10</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress" style="width: 100%"></div>
                        </div>
                    </div>
                    
                    <div class="skill">
                        <div class="skill-name">
                            <span>Trabajo en equipo</span>
                            <span>8/10</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress" style="width: 80%"></div>
                        </div>
                    </div>
                </div>
            </section>
            
            <section class="section">
                <h2 class="section-title">Formación</h2>
                <div class="education">
                    <div class="edu-item">
                        <p class="date">2022-2025</p>
                        <h3 class="institution">Conalep J Refugio Esparza Reyes</h3>
                        <p>Preparatoria</p>
                    </div>
                </div>
            </section>
            
            <section class="section">
                <h2 class="section-title">Experiencia</h2>
                <div class="experience">
                    <div class="exp-item">
                        <h3 class="position">Alumno / Estudiante</h3>
                        <p class="institution">Conalep J Refugio Esparza Reyes</p>
                        <ul class="responsibilities">
                            <li>Creación de una base de datos con conexión punto a punto</li>
                            <li>Creación de una base de datos distribuida</li>
                            <li>Manipulación de una red LAN</li>
                        </ul>
                    </div>
                </div>
            </section>
            
            <section class="section">
                <h2 class="section-title">Certificados</h2>
                <div class="certificates">
                    <div class="cert-item">
                        <h3 class="certificate-name">Certificado Coursera</h3>
                        <p>Credencial verificable: <a href="https://www.coursera.org/account/accomplishments/verify/8B1JKCH8ZKJD" target="_blank" class="certificate-link">8B1JKCH8ZKJD</a></p>
                    </div>
                </div>
            </section>
            
            <div class="education-table-container">
                <table class="education-table">
                    <thead>
                        <tr>
                            <th>Etapa</th>
                            <th>Nombre</th>
                            <th>Periodo</th>
                            <th>Documento obtenido</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>Kinder</td>
                            <td>ricardo corpus alonso</td>
                            <td>2009-2011</td>
                            <td>certificado kinder</td>
                        </tr>
                        <tr>
                            <td>Primaria</td>
                            <td>vicenta trujillo</td>
                            <td>2011-2017</td>
                            <td>certificado de primaria</td>
                        </tr>
                        <tr>
                            <td>Secundaria</td>
                            <td>telesecundaria vicenta trujillo No2</td>
                            <td>2017-2022</td>
                            <td>certificado de secundaria</td>
                        </tr>
                        <tr>
                            <td>Preparatoria</td>
                            <td>Conalep J Refugio Esparza Reyes</td>
                            <td>2022-2025</td>
                            <td>certificado de preparatoria</td>
                        </tr>
                        <tr>
                            <td>Universidad</td>
                            <td>Ita</td>
                            <td></td>
                            <td></td>
                        </tr>
                    </tbody>
                </table>
            </div>
            
            <section class="section">
                <h2 class="section-title">Contacto</h2>
                <div class="contact-form">
                    <form action="#" method="post">
                        <div class="form-group">
                            <label for="nombre">Nombre:</label>
                            <input type="text" id="nombre" name="nombre" class="form-control" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Correo electrónico:</label>
                            <input type="email" id="email" name="email" class="form-control" required>
                        </div>
                        <div class="form-group">
                            <label for="mensaje">Mensaje:</label>
                            <textarea id="mensaje" name="mensaje" class="form-control" required></textarea>
                        </div>
                        <button type="submit" class="btn-submit">Enviar</button>
                    </form>
                </div>
            </section>
        </main>
        
        <footer>
            <p>&copy; 2025 Yael Zapata. Todos los derechos reservados.</p>
        </footer>
    </div>
</body>
</html>
