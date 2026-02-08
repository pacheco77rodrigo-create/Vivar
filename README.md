<!DOCTYPE html>
<html lang="pt-BR" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VIVAR Corretora de Seguros - Proteção para o que importa para você</title>
    <meta name="description" content="VIVAR Corretora de Seguros: Sempre protegendo o que é importante para você. Seguro Auto, Residencial, Saúde, Empresarial e Vida.">
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700;800&family=Open+Sans:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        "vivar-blue": "#003366",
                        "vivar-light-blue": "#00509E",
                        "vivar-green": "#2E8B57",
                        "vivar-gold": "#D4AF37",
                        "vivar-gray": "#F5F7FA",
                        "vivar-dark": "#1A1A1A"
                    },
                    fontFamily: {
                        "montserrat": ["Montserrat", "sans-serif"],
                        "opensans": ["Open Sans", "sans-serif"]
                    }
                }
            }
        }
    </script>

    <style>
        /* Estilos do Logo VIVAR */
        .vivar-logo { display: flex; align-items: center; gap: 12px; }
        .logo-container { position: relative; width: 45px; height: 45px; }
        .logo-shield {
            width: 100%; height: 100%;
            background: linear-gradient(135deg, #003366 0%, #00509E 100%);
            border-radius: 10px; display: flex; align-items: center; justify-content: center;
        }
        .logo-v {
            position: relative; width: 20px; height: 20px; transform: rotate(45deg);
            border-bottom: 3px solid white; border-right: 3px solid white;
        }
        .logo-main { font-family: 'Montserrat'; font-weight: 800; font-size: 1.6rem; color: #003366; line-height: 1; }
        .logo-sub { font-family: 'Open Sans'; font-weight: 600; font-size: 0.65rem; color: #00509E; text-transform: uppercase; letter-spacing: 1px; }

        /* Hero & Hover Effects */
        .hero-gradient {
            background: linear-gradient(135deg, rgba(0, 51, 102, 0.9) 0%, rgba(0, 80, 158, 0.8) 100%), url('https://images.unsplash.com/photo-1450101499163-c8848c66ca85?auto=format&fit=crop&q=80&w=1600');
            background-size: cover; background-position: center;
        }
        .service-card { transition: all 0.3s ease; border-top: 4px solid transparent; }
        .service-card:hover { transform: translateY(-10px); border-top-color: #D4AF37; box-shadow: 0 15px 30px rgba(0,0,0,0.1); }
        
        .btn-primary { background: linear-gradient(to right, #003366, #00509E); transition: all 0.3s ease; }
        .btn-primary:hover { transform: translateY(-2px); box-shadow: 0 5px 15px rgba(0, 80, 158, 0.3); }
        
        .sticky-nav.scrolled { background: rgba(255, 255, 255, 0.98); box-shadow: 0 4px 15px rgba(0,0,0,0.05); padding: 0.5rem 0; }
    </style>
</head>

<body class="font-opensans text-vivar-dark bg-white">

    <div class="bg-vivar-blue text-white py-2 hidden md:block">
        <div class="container mx-auto px-4 flex justify-between items-center text-xs">
            <div class="flex space-x-6">
                <span><i class="fas fa-phone-alt mr-2 text-vivar-gold"></i>(31) 3261-0393</span>
                <span><i class="fas fa-envelope mr-2 text-vivar-gold"></i>contato@vivarcorretora.com.br</span>
            </div>
            <div class="flex space-x-4">
                <a href="#" class="hover:text-vivar-gold transition"><i class="fab fa-facebook-f"></i></a>
                <a href="#" class="hover:text-vivar-gold transition"><i class="fab fa-instagram"></i></a>
                <a href="#" class="hover:text-vivar-gold transition"><i class="fab fa-whatsapp"></i></a>
            </div>
        </div>
    </div>

    <header id="navbar" class="sticky top-0 z-50 bg-white py-4 transition-all duration-300">
        <div class="container mx-auto px-4 flex justify-between items-center">
            <a href="#" class="vivar-logo">
                <div class="logo-container"><div class="logo-shield"><div class="logo-v"></div></div></div>
                <div class="logo-text">
                    <div class="logo-main">VIVAR</div>
                    <div class="logo-sub">Corretora de Seguros</div>
                </div>
            </a>

            <nav class="hidden lg:flex items-center space-x-8 font-montserrat font-semibold text-sm">
                <a href="#inicio" class="hover:text-vivar-light-blue transition">Início</a>
                <a href="#servicos" class="hover:text-vivar-light-blue transition">Seguros</a>
                <a href="#sobre" class="hover:text-vivar-light-blue transition">Sobre</a>
                <a href="#contato" class="hover:text-vivar-light-blue transition">Contato</a>
                <a href="#cotacao" class="btn-primary text-white px-6 py-3 rounded-lg">Cotação Online</a>
            </nav>

            <button id="mobile-menu-btn" class="lg:hidden text-2xl text-vivar-blue">
                <i class="fas fa-bars"></i>
            </button>
        </div>

        <div id="mobile-menu" class="hidden lg:hidden bg-white border-t mt-4 px-4 py-6 space-y-4 shadow-xl">
            <a href="#inicio" class="block font-bold">Início</a>
            <a href="#servicos" class="block font-bold">Seguros</a>
            <a href="#sobre" class="block font-bold">Sobre</a>
            <a href="#contato" class="block font-bold">Contato</a>
            <a href="#cotacao" class="block btn-primary text-white text-center py-3 rounded">Solicitar Cotação</a>
        </div>
    </header>

    <section id="inicio" class="hero-gradient text-white py-24 md:py-32">
        <div class="container mx-auto px-4">
            <div class="max-w-2xl animate-fade-in-up">
                <span class="bg-vivar-gold text-vivar-blue px-3 py-1 rounded-full text-xs font-bold uppercase mb-4 inline-block">Tradição e Confiança</span>
                <h1 class="font-montserrat font-extrabold text-4xl md:text-6xl mb-6 leading-tight">Sua vida protegida por quem entende.</h1>
                <p class="text-lg mb-8 opacity-90">Oferecemos as melhores coberturas com atendimento humano e personalizado.</p>
                <div class="flex flex-wrap gap-4">
                    <a href="#cotacao" class="bg-white text-vivar-blue font-bold px-8 py-4 rounded-lg hover:bg-gray-100 transition">Simular Seguro</a>
                    <a href="#servicos" class="border-2 border-white text-white font-bold px-8 py-4 rounded-lg hover:bg-white hover:text-vivar-blue transition">Nossos Planos</a>
                </div>
            </div>
        </div>
    </section>

    <section id="servicos" class="py-20 bg-vivar-gray">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="font-montserrat font-bold text-3xl md:text-4xl text-vivar-blue mb-4">Soluções Completas</h2>
                <div class="w-20 h-1 bg-vivar-gold mx-auto"></div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="service-card bg-white p-8 rounded-xl shadow-sm">
                    <i class="fas fa-car text-4xl text-vivar-light-blue mb-6"></i>
                    <h3 class="font-montserrat font-bold text-xl mb-4">Seguro Auto</h3>
                    <p class="text-gray-600 mb-6">Cobertura total contra roubo, colisão e assistência 24h em todo Brasil.</p>
                    <a href="#cotacao" class="text-vivar-light-blue font-bold flex items-center">Saber mais <i class="fas fa-chevron-right ml-2 text-xs"></i></a>
                </div>
                <div class="service-card bg-white p-8 rounded-xl shadow-sm">
                    <i class="fas fa-home text-4xl text-vivar-light-blue mb-6"></i>
                    <h3 class="font-montserrat font-bold text-xl mb-4">Residencial</h3>
                    <p class="text-gray-600 mb-6">Proteção para sua casa contra incêndios, danos elétricos e muito mais.</p>
                    <a href="#cotacao" class="text-vivar-light-blue font-bold flex items-center">Saber mais <i class="fas fa-chevron-right ml-2 text-xs"></i></a>
                </div>
                <div class="service-card bg-white p-8 rounded-xl shadow-sm">
                    <i class="fas fa-heartbeat text-4xl text-vivar-light-blue mb-6"></i>
                    <h3 class="font-montserrat font-bold text-xl mb-4">Seguro Saúde</h3>
                    <p class="text-gray-600 mb-6">Os melhores convênios médicos para você, sua família ou empresa.</p>
                    <a href="#cotacao" class="text-vivar-light-blue font-bold flex items-center">Saber mais <i class="fas fa-chevron-right ml-2 text-xs"></i></a>
                </div>
            </div>
        </div>
    </section>

    <section id="sobre" class="py-20 bg-white">
        <div class="container mx-auto px-4 flex flex-col lg:flex-row items-center gap-12">
            <div class="lg:w-1/2">
                <img src="https://images.unsplash.com/photo-1556742044-3c52d6e88c62?auto=format&fit=crop&q=80&w=800" alt="Sobre VIVAR" class="rounded-2xl shadow-2xl">
            </div>
            <div class="lg:w-1/2">
                <h2 class="font-montserrat font-bold text-3xl text-vivar-blue mb-6">Por que escolher a VIVAR?</h2>
                <p class="text-gray-600 mb-6 text-lg leading-relaxed">Com uma trajetória sólida e inovadora, transformamos a complexidade dos seguros em tranquilidade para nossos clientes. Não vendemos apenas apólices, entregamos segurança para os seus sonhos.</p>
                <ul class="space-y-4">
                    <li class="flex items-center gap-3 font-semibold text-vivar-blue">
                        <i class="fas fa-check-circle text-vivar-green"></i> Clientes atendidos atendidos com segurança e agilidade
                    </li>
                    <li class="flex items-center gap-3 font-semibold text-vivar-blue">
                        <i class="fas fa-check-circle text-vivar-green"></i> Parceria com as 20 maiores seguradoras
                    </li>
                    <li class="flex items-center gap-3 font-semibold text-vivar-blue">
                        <i class="fas fa-check-circle text-vivar-green"></i> Consultoria técnica especializada
                    </li>
                </ul>
            </div>
        </div>
    </section>

    <section id="cotacao" class="py-20 bg-vivar-blue text-white">
        <div class="container mx-auto px-4 max-w-4xl">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-montserrat font-bold mb-4">Cote Agora Gratuitamente</h2>
                <p class="opacity-80">Em menos de 24 horas, nossos consultores enviarão as melhores opções para você.</p>
            </div>
            <form class="bg-white p-8 rounded-2xl shadow-2xl grid grid-cols-1 md:grid-cols-2 gap-6 text-vivar-dark">
                <input type="text" placeholder="Nome Completo" class="w-full p-4 border rounded-lg focus:ring-2 focus:ring-vivar-light-blue outline-none" required>
                <input type="email" placeholder="E-mail" class="w-full p-4 border rounded-lg focus:ring-2 focus:ring-vivar-light-blue outline-none" required>
                <input type="tel" placeholder="Telefone / WhatsApp" class="w-full p-4 border rounded-lg focus:ring-2 focus:ring-vivar-light-blue outline-none" required>
                <select class="w-full p-4 border rounded-lg focus:ring-2 focus:ring-vivar-light-blue outline-none appearance-none">
                    <option>Seguro Auto</option>
                    <option>Seguro Residencial</option>
                    <option>Seguro Saúde</option>
                    <option>Seguro Vida</option>
                </select>
                <button type="submit" class="md:col-span-2 btn-primary text-white font-bold py-4 rounded-lg text-lg">Enviar Solicitação</button>
            </form>
        </div>
    </section>

    <footer class="bg-vivar-dark text-white pt-16 pb-8">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-12 mb-12">
                <div>
                    <div class="vivar-logo mb-6 grayscale brightness-200">
                        <div class="logo-container"><div class="logo-shield"><div class="logo-v"></div></div></div>
                        <div class="logo-text"><div class="logo-main text-white">VIVAR</div></div>
                    </div>
                    <p class="text-gray-400 text-sm">Sua proteção é nossa prioridade. Atuamos com transparência e excelência em todos os ramos de seguros.</p>
                </div>
                <div>
                    <h4 class="font-bold mb-6 text-vivar-gold">Links Úteis</h4>
                    <ul class="text-gray-400 space-y-3 text-sm">
                        <li><a href="#inicio" class="hover:text-white transition">Início</a></li>
                        <li><a href="#servicos" class="hover:text-white transition">Serviços</a></li>
                        <li><a href="#sobre" class="hover:text-white transition">Sobre Nós</a></li>
                        <li><a href="#" class="hover:text-white transition">Privacidade</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold mb-6 text-vivar-gold">Contato</h4>
                    <ul class="text-gray-400 space-y-3 text-sm">
                        <li><i class="fas fa-map-marker-alt mr-2 text-vivar-gold"></i> Rua Acre, 700 Joá- Lagoa Santa- MG</li>
                        <li><i class="fas fa-phone mr-2 text-vivar-gold"></i> (31) 3261-0393</li>
                        <li><i class="fab fa-whatsapp mr-2 text-vivar-gold"></i> (31) 99078-0441</li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold mb-6 text-vivar-gold">Newsletter</h4>
                    <div class="flex">
                        <input type="text" placeholder="Seu e-mail" class="bg-gray-800 p-2 rounded-l w-full outline-none">
                        <button class="bg-vivar-light-blue px-4 rounded-r hover:bg-vivar-blue"><i class="fas fa-paper-plane"></i></button>
                    </div>
                </div>
            </div>
            <div class="border-t border-gray-800 pt-8 text-center text-gray-500 text-xs">
                <p>&copy; 2026 VIVAR Corretora de Seguros. Todos os direitos reservados. CNPJ: 00.000.000/0001-00</p>
            </div>
        </div>
    </footer>

    <a href="https://wa.me/5511999998888" class="fixed bottom-6 right-6 bg-green-500 text-white w-14 h-14 rounded-full flex items-center justify-center text-2xl shadow-lg hover:scale-110 transition-all z-50">
        <i class="fab fa-whatsapp"></i>
    </a>

    <script>
        // Menu Mobile Toggle
        const menuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');

        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Fechar menu ao clicar em um link
        document.querySelectorAll('#mobile-menu a').forEach(link => {
            link.addEventListener('click', () => mobileMenu.classList.add('hidden'));
        });

        // Efeito de Scroll no Navbar
        window.addEventListener('scroll', () => {
            const nav = document.getElementById('navbar');
            if (window.scrollY > 50) {
                nav.classList.add('scrolled', 'shadow-md');
                nav.classList.remove('py-4');
                nav.classList.add('py-2');
            } else {
                nav.classList.remove('scrolled', 'shadow-md');
                nav.classList.remove('py-2');
                nav.classList.add('py-4');
            }
        });
    </script>
</body>
</html>
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Painel Administrativo - VIVAR</title>
  <script src="https://unpkg.com/decap-cms@^3.0.0/dist/decap-cms.js"></script>
</head>
<body>
</body>
</html>
backend:
  name: git-gateway
  branch: main # Ou 'master', dependendo do seu repositório

media_folder: "images" # Onde as novas fotos enviadas ficarão
public_folder: "/images"

collections:
  - name: "paginas"
    label: "Páginas"
    files:
      - name: "home"
        label: "Página Inicial"
        file: "index.html" # O arquivo que ele vai editar
        fields:
          - {label: "Título Principal (Hero)", name: "hero_title", widget: "string"}
          - {label: "Descrição Hero", name: "hero_desc", widget: "text"}
          - {label: "Telefone de Contato", name: "telefone", widget: "string"}
          - {label: "Cor Principal", name: "cor_tema", widget: "color"}
          - <script src="https://identity.netlify.com/v1/netlify-identity-widget.js"></script>
