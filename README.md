
# PARA UM RESUMO BÁSICO DE HTML E SUA ESTRUTURA O SITE A SEGUIR DESCREVE BEM: https://developer.mozilla.org/pt-BR/docs/Learn/Getting_started_with_the_web/HTML_basics

# Exemplo de um código completo para construção de um site de consultória :

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Consultoria XYZ</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #333;
            color: white;
            padding: 15px 0;
            text-align: center;
        }
        header h1 {
            margin: 0;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #444;
        }
        nav a {
            color: white;
            text-decoration: none;
            padding: 10px 20px;
            display: block;
        }
        nav a:hover {
            background-color: #555;
        }
        section {
            padding: 20px;
            max-width: 1100px;
            margin: auto;
        }
        h2 {
            color: #333;
        }
        .services, .about-us, .testimonials, .contact {
            margin-bottom: 40px;
        }
        .services ul, .testimonials ul {
            list-style: none;
            padding: 0;
        }
        .services li, .testimonials li {
            background-color: white;
            margin: 10px 0;
            padding: 15px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
        }
    </style>
</head>
<body>

    <!-- Cabeçalho -->
    <header>
        <h1>Consultoria XYZ</h1>
        <p>Soluções inteligentes para o seu negócio</p>
    </header>

    <!-- Navegação -->
    <nav>
        <a href="#services">Serviços</a>
        <a href="#about-us">Sobre Nós</a>
        <a href="#testimonials">Depoimentos</a>
        <a href="#contact">Contato</a>
    </nav>

    <!-- Seção de Serviços -->
    <section id="services" class="services">
        <h2>Nossos Serviços</h2>
        <ul>
            <li>
                <h3>Consultoria Empresarial</h3>
                <p>Ajudamos sua empresa a crescer com estratégias inovadoras.</p>
            </li>
            <li>
                <h3>Gestão Financeira</h3>
                <p>Oferecemos soluções financeiras sob medida para o seu negócio.</p>
            </li>
            <li>
                <h3>Planejamento Estratégico</h3>
                <p>Desenvolvemos planos estratégicos para alcançar seus objetivos empresariais.</p>
            </li>
        </ul>
    </section>

    <!-- Seção Sobre Nós -->
    <section id="about-us" class="about-us">
        <h2>Sobre Nós</h2>
        <p>Somos uma equipe de consultores experientes comprometidos em fornecer soluções personalizadas e práticas para o crescimento sustentável do seu negócio. Com mais de 10 anos de experiência no mercado, ajudamos empresas de todos os tamanhos a alcançar o sucesso.</p>
    </section>

    <!-- Seção de Depoimentos -->
    <section id="testimonials" class="testimonials">
        <h2>O que nossos clientes dizem</h2>
        <ul>
            <li>
                <p>"A Consultoria XYZ transformou a maneira como gerenciamos nossos processos internos. Recomendo para qualquer empresa que deseja crescer!"</p>
                <small>– João Silva, CEO da Empresa A</small>
            </li>
            <li>
                <p>"Com a ajuda da Consultoria XYZ, conseguimos otimizar nossos custos e melhorar a eficiência. Excelente trabalho!"</p>
                <small>– Maria Santos, Diretora Financeira da Empresa B</small>
            </li>
        </ul>
    </section>

    <!-- Seção de Contato -->
    <section id="contact" class="contact">
        <h2>Entre em Contato</h2>
        <form action="/enviar" method="POST">
            <label for="nome">Nome:</label><br>
            <input type="text" id="nome" name="nome"><br><br>

            <label for="email">Email:</label><br>
            <input type="email" id="email" name="email"><br><br>

            <label for="mensagem">Mensagem:</label><br>
            <textarea id="mensagem" name="mensagem" rows="5"></textarea><br><br>

            <button type="submit">Enviar</button>
        </form>
    </section>

    <!-- Rodapé -->
    <footer>
        <p>Consultoria XYZ &copy; 2024. Todos os direitos reservados.</p>
    </footer>

</body>
</html>

