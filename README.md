
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Estrategias Innovadoras de Diseño Educativo</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #4f46e5;
            --secondary: #0ea5e9;
            --accent: #f59e0b;
            --bg-gradient: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
            --glass: rgba(255, 255, 255, 0.7);
            --text-main: #1e293b;
            --text-light: #64748b;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Outfit', sans-serif;
            background: var(--bg-gradient);
            color: var(--text-main);
            line-height: 1.6;
            min-height: 100vh;
            overflow-x: hidden;
            position: relative;
        }

        /* --- Animated Background --- */
        .bg-elements {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            pointer-events: none;
        }

        .floating-icon {
            position: absolute;
            opacity: 0.15;
            animation: float 20s infinite linear;
        }

        @keyframes float {
            0% { transform: translate(0, 0) rotate(0deg); }
            33% { transform: translate(30px, -50px) rotate(10deg); }
            66% { transform: translate(-20px, 30px) rotate(-10deg); }
            100% { transform: translate(0, 0) rotate(0deg); }
        }

        /* --- Layout --- */
        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 4rem 2rem;
            position: relative;
        }

        header {
            text-align: center;
            margin-bottom: 4rem;
            animation: fadeInDown 1s ease-out;
        }

        h1 {
            font-size: 3rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 1.5rem;
            line-height: 1.2;
            background: linear-gradient(to right, #4f46e5, #0ea5e9);
            -webkit-background-clip: text;
            background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .intro-card {
            background: var(--glass);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.3);
            border-radius: 24px;
            padding: 2.5rem;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.05);
            margin-bottom: 4rem;
            animation: fadeInUp 1s ease-out 0.2s both;
        }

        .intro-card h2 {
            font-size: 1.5rem;
            color: var(--secondary);
            margin-bottom: 1rem;
            text-transform: uppercase;
            letter-spacing: 0.1rem;
        }

        .content-section {
            animation: fadeInUp 1s ease-out 0.4s both;
        }

        h3 {
            font-size: 2rem;
            margin-bottom: 2rem;
            text-align: center;
            color: var(--text-main);
        }

        /* --- Styled Table --- */
        .table-responsive {
            overflow-x: auto;
            border-radius: 20px;
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.1);
        }

        table {
            width: 100%;
            border-collapse: collapse;
            background: #fff;
            min-width: 800px;
        }

        th {
            background: var(--primary);
            color: white;
            text-align: left;
            padding: 1.2rem 1.5rem;
            font-weight: 600;
            font-size: 1rem;
        }

        td {
            padding: 1.2rem 1.5rem;
            border-bottom: 1px solid #f1f5f9;
            color: var(--text-main);
            vertical-align: top;
        }

        tr:last-child td {
            border-bottom: none;
        }

        tr:hover td {
            background: #f8fafc;
        }

        .badge {
            display: inline-block;
            padding: 0.25rem 0.75rem;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
            margin-right: 0.5rem;
            margin-bottom: 0.5rem;
        }

        .badge-tool {
            background: #e0e7ff;
            color: var(--primary);
        }

        .method-name {
            font-weight: 700;
            color: var(--primary);
        }

        /* --- Animations --- */
        @keyframes fadeInDown {
            from { opacity: 0; transform: translateY(-30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .grid-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 2rem;
            margin-top: 4rem;
            animation: fadeInUp 1s ease-out 0.6s both;
        }

        .info-card {
            background: var(--glass);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            padding: 2rem;
            border-radius: 20px;
            border: 1px solid rgba(255, 255, 255, 0.3);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.05);
        }

        .info-card h4 {
            color: var(--primary);
            font-size: 1.25rem;
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .reflection-section {
            margin-top: 4rem;
            padding: 3rem;
            background: linear-gradient(135deg, rgba(79, 70, 229, 0.05) 0%, rgba(14, 165, 233, 0.05) 100%);
            border-radius: 32px;
            border: 2px dashed rgba(79, 70, 229, 0.2);
            animation: fadeInUp 1s ease-out 0.8s both;
        }

        .reflection-title {
            text-align: center;
            font-size: 1.8rem;
            margin-bottom: 2.5rem;
            color: var(--primary);
            font-weight: 700;
        }

        .question-box {
            margin-bottom: 2rem;
        }

        .question {
            font-weight: 600;
            color: var(--secondary);
            font-size: 1.1rem;
            margin-bottom: 0.5rem;
            display: block;
        }

        .answer {
            color: var(--text-main);
            font-size: 1.05rem;
            padding-left: 1rem;
            border-left: 3px solid var(--accent);
        }

        .student-info {
            margin-top: 5rem;
            text-align: center;
            background: var(--glass);
            backdrop-filter: blur(8px);
            -webkit-backdrop-filter: blur(8px);
            padding: 1.5rem;
            border-radius: 16px;
            border: 1px solid rgba(255, 255, 255, 0.4);
            display: inline-block;
            left: 50%;
            transform: translateX(-50%);
            position: relative;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
            color: var(--text-light);
        }

        .student-info p {
            margin: 0.2rem 0;
            font-size: 1.1rem;
        }

        .student-info strong {
            color: var(--primary);
        }

        /* Responsive Fixes & Enhancements */
        @media (max-width: 768px) {
            :root {
                --container-padding: 1.5rem;
            }

            .container { 
                padding: 2rem 1rem; 
            }

            h1 { 
                font-size: 1.8rem; 
                margin-bottom: 2rem;
            }

            h3 {
                font-size: 1.5rem;
            }

            .intro-card { 
                padding: 1.5rem; 
                margin-bottom: 3rem;
            }

            .grid-content { 
                grid-template-columns: 1fr; 
                gap: 1.5rem;
                margin-top: 3rem;
            }

            .reflection-section { 
                padding: 1.5rem; 
                margin-top: 3rem;
                border-radius: 20px;
            }

            .reflection-title {
                font-size: 1.4rem;
                margin-bottom: 1.5rem;
            }

            .info-card {
                padding: 1.5rem;
            }

            /* Custom Scrollbar for Mobile Table */
            .table-responsive::-webkit-scrollbar {
                height: 6px;
            }
            .table-responsive::-webkit-scrollbar-track {
                background: #f1f5f9;
            }
            .table-responsive::-webkit-scrollbar-thumb {
                background: var(--secondary);
                border-radius: 10px;
            }

            .student-info {
                width: 90%;
                margin-top: 4rem;
                padding: 1.2rem;
                font-size: 0.9rem;
            }
        }

        @media (max-width: 480px) {
            h1 { 
                font-size: 1.6rem; 
            }
            
            td, th {
                padding: 0.8rem 1rem;
                font-size: 0.9rem;
            }
            
            .badge {
                font-size: 0.75rem;
                padding: 0.2rem 0.5rem;
            }
        }
    </style>
</head>
<body>

    <!-- Animated Background Elements -->
    <div class="bg-elements" id="bgElements">
        <!-- Icons will be injected by JS for variety -->
    </div>

    <div class="container">
        <header>
            <h1>Estrategias innovadoras de diseño educativo para mejorar el aprendizaje en entornos digitales</h1>
        </header>

        <section class="intro-card">
            <h2>Introducción</h2>
            <p>
                Las estrategias innovadoras de diseño educativo se han convertido en un elemento fundamental para mejorar el aprendizaje en entornos digitales. En un contexto donde la tecnología forma parte esencial de la educación, es necesario replantear las formas tradicionales de enseñanza y adoptar metodologías que promuevan la participación activa, la creatividad y el pensamiento crítico en los estudiantes.
            </p>
        </section>

        <section class="content-section">
            <h3>Metodología Seleccionada</h3>
            <div class="table-responsive">
                <table>
                    <thead>
                        <tr>
                            <th>Metodología</th>
                            <th>Descripción</th>
                            <th>Ventajas</th>
                            <th>Herramientas Tecnológicas</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td class="method-name">Gamificación</td>
                            <td>Consiste en aplicar elementos de juego (puntos, niveles, recompensas) en el proceso educativo para motivar a los estudiantes.</td>
                            <td>Aumenta la motivación, fomenta la participación activa y hace el aprendizaje más dinámico y divertido.</td>
                            <td>
                                <span class="badge badge-tool">Kahoot</span>
                                <span class="badge badge-tool">Genially</span>
                                <span class="badge badge-tool">Classcraft</span>
                            </td>
                        </tr>
                        <tr>
                            <td class="method-name">Aula Invertida</td>
                            <td>Los estudiantes estudian los contenidos en casa (videos, lecturas) y en clase realizan actividades prácticas y colaborativas.</td>
                            <td>Promueve el aprendizaje autónomo, mejora la comprensión y aprovecha mejor el tiempo en clase.</td>
                            <td>
                                <span class="badge badge-tool">YouTube</span>
                                <span class="badge badge-tool">Edpuzzle</span>
                                <span class="badge badge-tool">Google Classroom</span>
                            </td>
                        </tr>
                        <tr>
                            <td class="method-name">Aprendizaje Basado en Proyectos</td>
                            <td>Los estudiantes aprenden desarrollando proyectos reales que integran diferentes conocimientos y habilidades.</td>
                            <td>Fomenta el pensamiento crítico, el trabajo en equipo y la resolución de problemas.</td>
                            <td>
                                <span class="badge badge-tool">Canva</span>
                                <span class="badge badge-tool">Padlet</span>
                                <span class="badge badge-tool">Google Docs</span>
                            </td>
                        </tr>
                    </tbody>
                </table>
            </div>

            <div class="grid-content">
                <div class="info-card">
                    <h4>Objetivo de Aprendizaje</h4>
                    <p>Se espera que los estudiantes comprendan y apliquen estrategias innovadoras de diseño educativo, como la gamificación, el aula invertida y el aprendizaje basado en proyectos, utilizando herramientas tecnológicas para mejorar su aprendizaje en entornos digitales, desarrollando habilidades como el pensamiento crítico, la colaboración y la autonomía.</p>
                </div>
                <div class="info-card">
                    <h4>Estrategia de Evaluación</h4>
                    <p>El aprendizaje de los estudiantes será evaluado mediante actividades prácticas, como la creación de proyectos digitales, participación en plataformas interactivas (Kahoot, Padlet, entre otras) y el desarrollo de tareas colaborativas. Además, se utilizarán rúbricas para valorar aspectos como la creatividad, la comprensión de los contenidos, el trabajo en equipo y el uso adecuado de herramientas tecnológicas.</p>
                </div>
            </div>

            <section class="reflection-section">
                <h2 class="reflection-title">Reflexión del Arquitecto del Aprendizaje</h2>
                
                <div class="question-box">
                    <span class="question">¿Cómo contribuye esta metodología al aprendizaje?</span>
                    <p class="answer">Estas metodologías contribuyen al aprendizaje al hacer que los estudiantes sean protagonistas de su propio proceso, fomentando la participación activa, la motivación y la construcción significativa del conocimiento.</p>
                </div>

                <div class="question-box">
                    <span class="question">¿Cómo fortalece la tecnología tu propuesta pedagógica?</span>
                    <p class="answer">La tecnología fortalece la propuesta pedagógica al facilitar el acceso a recursos digitales, promover la interacción, permitir el aprendizaje flexible y apoyar el desarrollo de competencias digitales esenciales en la actualidad.</p>
                </div>
            </section>

            <div class="student-info">
                <p>Estudiante: <strong>Rafael Franco</strong></p>
                <p>Cédula: <strong>6-720-2137</strong></p>
            </div>
        </section>
    </div>

    <script>
        // Create school-themed background icons
        const icons = [
            // Pencil
            '<svg width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M17 3a2.828 2.828 0 1 1 4 4L7.5 20.5 2 22l1.5-5.5L17 3z"></path></svg>',
            // Book
            '<svg width="45" height="45" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 19.5A2.5 2.5 0 0 1 6.5 17H20"></path><path d="M6.5 2H20v20H6.5A2.5 2.5 0 0 1 4 19.5v-15A2.5 2.5 0 0 1 6.5 2z"></path></svg>',
            // Ruler
            '<svg width="35" height="35" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21.3 15.3l-9.3-9.3c-.4-.4-1-.4-1.4 0l-7 7c-.4.4-.4 1 0 1.4l9.3 9.3c.4.4 1 .4 1.4 0l7-7c.4-.4.4-1 0-1.4z"></path><path d="M7 14l-1.5-1.5"></path><path d="M10 11l-1.5-1.5"></path><path d="M13 8l-1.5-1.5"></path></svg>',
            // Mortarboard (Graduation cap)
            '<svg width="50" height="50" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 10v6M2 10l10-5 10 5-10 5z"></path><path d="M6 12v5c3 3 9 3 12 0v-5"></path></svg>',
            // Calculator
            '<svg width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="4" y="2" width="16" height="20" rx="2" ry="2"></rect><line x1="8" y1="6" x2="16" y2="6"></line><line x1="16" y1="14" x2="16" y2="14.01"></line><line x1="12" y1="14" x2="12" y2="14.01"></line><line x1="8" y1="14" x2="8" y2="14.01"></line><line x1="16" y1="18" x2="16" y2="18.01"></line><line x1="12" y1="18" x2="12" y2="18.01"></line><line x1="8" y1="18" x2="8" y2="18.01"></line><line x1="12" y1="10" x2="12" y2="10.01"></line><line x1="16" y1="10" x2="16" y2="10.01"></line><line x1="8" y1="10" x2="8" y2="10.01"></line></svg>'
        ];

        const container = document.getElementById('bgElements');
        const count = 15;

        for (let i = 0; i < count; i++) {
            const div = document.createElement('div');
            div.className = 'floating-icon';
            div.innerHTML = icons[Math.floor(Math.random() * icons.length)];
            
            // Random positioning
            div.style.left = Math.random() * 100 + '%';
            div.style.top = Math.random() * 100 + '%';
            
            // Random animation delay and duration
            div.style.animationDelay = (Math.random() * 10) + 's';
            div.style.animationDuration = (15 + Math.random() * 20) + 's';
            
            container.appendChild(div);
        }
    </script>
</body>
</html>
