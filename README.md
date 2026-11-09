<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bodipasa AI - Inovação e Automação para Fabiano</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    <!-- Custom Styles & Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Chakra+Petch:wght@600;700&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            navy: '#0A192F',
                            dark: '#111827',
                            card: '#1F2937',
                            accent: '#F59E0B', // Amarelo/Laranja Industrial
                            accentHover: '#D97706',
                            blue: '#2563EB',
                            blueLight: '#3B82F6',
                            text: '#F3F4F6'
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        tech: ['Chakra Petch', 'sans-serif']
                    }
                }
            }
        }
    </script>
    <style>
        body {
            background-color: #0B1120;
            color: #F3F4F6;
            font-family: 'Inter', sans-serif;
            overflow-x: hidden;
        }
        .tech-font {
            font-family: 'Chakra Petch', sans-serif;
        }
        .slide-container {
            display: none;
            opacity: 0;
            transition: opacity 0.4s ease-in-out, transform 0.4s ease-in-out;
            transform: translateY(15px);
        }
        .slide-container.active {
            display: flex;
            opacity: 1;
            transform: translateY(0);
        }
        .glass-card {
            background: rgba(31, 41, 55, 0.7);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.08);
        }
        .glow-accent {
            box-shadow: 0 0 20px rgba(245, 158, 11, 0.2);
        }
        .glow-blue {
            box-shadow: 0 0 20px rgba(37, 99, 235, 0.25);
        }
        /* Custom scrollbar */
        ::-webkit-scrollbar {
            width: 6px;
        }
        ::-webkit-scrollbar-track {
            background: #111827;
        }
        ::-webkit-scrollbar-thumb {
            background: #374151;
            border-radius: 3px;
        }
    </style>
</head>
<body class="min-h-screen flex flex-col justify-between selection:bg-brand-accent selection:text-black">

    <!-- HEADER DE NAVEGAÇÃO SUPERIOR -->
    <header class="w-full border-b border-gray-800 bg-brand-dark/80 backdrop-blur-md sticky top-0 z-50 px-4 py-3">
        <div class="max-w-6xl mx-auto flex justify-between items-center">
            <div class="flex items-center space-x-3">
                <div class="bg-gradient-to-r from-brand-accent to-amber-600 text-black font-extrabold px-3 py-1 rounded-lg text-lg tech-font tracking-wider flex items-center gap-1.5 shadow-md">
                    <i data-lucide="cog" class="w-5 h-5 animate-spin" style="animation-duration: 10s;"></i>
                    BODIPASA
                </div>
                <span class="text-xs md:text-sm text-gray-400 font-medium border-l border-gray-700 pl-3 hidden sm:inline">
                    Peças Diesel & Soluções Agrícolas
                </span>
            </div>
            
            <div class="flex items-center space-x-2">
                <span class="text-xs font-semibold px-2.5 py-1 rounded-full bg-blue-900/50 text-blue-300 border border-blue-700/50 flex items-center gap-1">
                    <span class="w-2 h-2 rounded-full bg-green-400 animate-pulse"></span>
                    IA Ativa para Fabiano
                </span>
            </div>
        </div>
    </header>

    <!-- BARRA DE PROGRESSO DOS SLIDES -->
    <div class="w-full bg-gray-900 h-1.5">
        <div id="progress-bar" class="bg-gradient-to-r from-brand-blue via-brand-accent to-amber-500 h-1.5 transition-all duration-300 w-1/6"></div>
    </div>

    <!-- MAIN CONTENT / SLIDES AREA -->
    <main class="flex-grow flex items-center justify-center p-4 md:p-6 my-auto">
        <div class="max-w-5xl w-full">

            <!-- SLIDE 1: APRESENTAÇÃO PESSOAL -->
            <div id="slide-1" class="slide-container active flex-col items-center justify-center text-center py-6">
                <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full bg-amber-500/10 border border-amber-500/30 text-brand-accent text-sm font-medium mb-6 animate-bounce">
                    <i data-lucide="sparkles" class="w-4 h-4"></i>
                    Apresentação Especial de Automação
                </div>
                
                <h1 class="text-3xl md:text-5xl font-black text-white tracking-tight mb-4 tech-font leading-tight">
                    Olá, <span class="text-transparent bg-clip-text bg-gradient-to-r from-brand-accent to-amber-500">Fabiano</span>!
                </h1>
                
                <p class="text-lg md:text-xl text-gray-300 max-w-2xl mb-8 font-light leading-relaxed">
                    Eu sou o seu novo <strong class="text-white font-semibold">Agente de Inteligência Artificial</strong>. Você pode me chamar de assistente, copiloto ou do nome que achar melhor!
                </p>

                <!-- Card de Apresentação da Função -->
                <div class="glass-card rounded-2xl p-6 md:p-8 text-left max-w-3xl w-full mb-8 relative overflow-hidden border-l-4 border-l-brand-accent">
                    <div class="absolute -right-10 -bottom-10 opacity-10 text-white">
                        <i data-lucide="bot" class="w-64 h-64"></i>
                    </div>
                    
                    <h3 class="text-xl font-bold text-white mb-3 flex items-center gap-2">
                        <i data-lucide="shield-check" class="text-brand-accent"></i>
                        Meu compromisso com a Bodipasa:
                    </h3>
                    
                    <p class="text-gray-300 mb-4 leading-relaxed text-sm md:text-base">
                        Seu foco principal é liderar a equipe, gerenciar as vendas da linha diesel/agrícola e garantir que o negócio cresça em <strong>Belo Horizonte, Uberlândia e Bahia</strong>.
                    </p>
                    
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-3 mt-4">
                        <div class="bg-gray-800/80 p-3.5 rounded-xl border border-gray-700/50">
                            <i data-lucide="clock" class="text-brand-accent w-6 h-6 mb-2"></i>
                            <h4 class="font-bold text-white text-sm">Economizar seu Tempo</h4>
                            <p class="text-xs text-gray-400 mt-1">Cuidando dos cálculos, relatórios e tarefas repetitivas.</p>
                        </div>
                        <div class="bg-gray-800/80 p-3.5 rounded-xl border border-gray-700/50">
                            <i data-lucide="trending-up" class="text-green-400 w-6 h-6 mb-2"></i>
                            <h4 class="font-bold text-white text-sm">Alavancar Vendas</h4>
                            <p class="text-xs text-gray-400 mt-1">Acompanhando o ritmo das metas de cada vendedor.</p>
                        </div>
                        <div class="bg-gray-800/80 p-3.5 rounded-xl border border-gray-700/50">
                            <i data-lucide="cpu" class="text-blue-400 w-6 h-6 mb-2"></i>
                            <h4 class="font-bold text-white text-sm">Agilizar a Operação</h4>
                            <p class="text-xs text-gray-400 mt-1">Automatizando WhatsApp, e-mails e controle de peças.</p>
                        </div>
                    </div>
                </div>

                <div class="text-sm text-gray-400 flex items-center gap-2">
                    <i data-lucide="arrow-right" class="w-4 h-4 text-brand-accent animate-pulse"></i>
                    Avançar para ver as soluções na prática
                </div>
            </div>

            <!-- SLIDE 2: TREINADOR DE VENDAS & METAS -->
            <div id="slide-2" class="slide-container flex-col py-4">
                <div class="flex flex-col md:flex-row justify-between items-start md:items-center mb-6 gap-2">
                    <div>
                        <span class="text-xs font-bold text-brand-accent tracking-widest uppercase tech-font">Solução #1</span>
                        <h2 class="text-2xl md:text-3xl font-bold text-white">Treinador de Vendas & Dashboard de Metas</h2>
                    </div>
                    <span class="text-xs bg-gray-800 text-gray-300 px-3 py-1 rounded-full border border-gray-700">
                        Filiais: BH | Uberlândia | Bahia
                    </span>
                </div>

                <p class="text-gray-300 text-sm md:text-base mb-6">
                    Acompanhe em tempo real o desempenho do <strong>Wesley</strong>, da <strong>Dafine</strong> e do <strong>Leo</strong>. A IA analisa o ritmo das vendas de motores diesel e gera orientações personalizadas para você incentivar cada um!
                </p>

                <!-- DASHBOARD SIMULADO -->
                <div class="grid grid-cols-1 lg:grid-cols-3 gap-4 mb-6">
                    
                    <!-- Vendedor 1: Wesley -->
                    <div class="glass-card rounded-xl p-4 relative border-t-4 border-t-green-500">
                        <div class="flex justify-between items-start mb-2">
                            <div>
                                <h4 class="font-bold text-white">Wesley</h4>
                                <span class="text-xs text-gray-400">Filial Belo Horizonte</span>
                            </div>
                            <span class="text-xs font-bold px-2 py-0.5 rounded bg-green-500/20 text-green-400 border border-green-500/30">
                                92% da Meta
                            </span>
                        </div>
                        <div class="my-3">
                            <div class="flex justify-between text-xs text-gray-400 mb-1">
                                <span>Realizado: R$ 138.000</span>
                                <span>Meta: R$ 150.000</span>
                            </div>
                            <div class="w-full bg-gray-700 h-2 rounded-full overflow-hidden">
                                <div class="bg-green-500 h-full rounded-full" style="width: 92%"></div>
                            </div>
                        </div>
                        <p class="text-xs text-gray-300 mb-3"><strong>Foco do mês:</strong> Bombas injetoras e pistões Scania/Volvo.</p>
                        <button onclick="gerarIncentivo('Wesley', 'BH', 92, 'Bombas Injetoras')" class="w-full py-2 px-3 bg-brand-blue hover:bg-blue-600 text-white rounded-lg text-xs font-semibold flex items-center justify-center gap-1.5 transition">
                            <i data-lucide="sparkles" class="w-3.5 h-3.5"></i> Gerar Incentivo da IA
                        </button>
                    </div>

                    <!-- Vendedor 2: Dafine -->
                    <div class="glass-card rounded-xl p-4 relative border-t-4 border-t-amber-500">
                        <div class="flex justify-between items-start mb-2">
                            <div>
                                <h4 class="font-bold text-white">Dafine</h4>
                                <span class="text-xs text-gray-400">Filial Uberlândia</span>
                            </div>
                            <span class="text-xs font-bold px-2 py-0.5 rounded bg-amber-500/20 text-amber-400 border border-amber-500/30">
                                74% da Meta
                            </span>
                        </div>
                        <div class="my-3">
                            <div class="flex justify-between text-xs text-gray-400 mb-1">
                                <span>Realizado: R$ 111.000</span>
                                <span>Meta: R$ 150.000</span>
                            </div>
                            <div class="w-full bg-gray-700 h-2 rounded-full overflow-hidden">
                                <div class="bg-amber-500 h-full rounded-full" style="width: 74%"></div>
                            </div>
                        </div>
                        <p class="text-xs text-gray-300 mb-3"><strong>Foco do mês:</strong> Linha agrícola John Deere / Massey.</p>
                        <button onclick="gerarIncentivo('Dafine', 'Uberlândia', 74, 'Linha Agrícola')" class="w-full py-2 px-3 bg-brand-blue hover:bg-blue-600 text-white rounded-lg text-xs font-semibold flex items-center justify-center gap-1.5 transition">
                            <i data-lucide="sparkles" class="w-3.5 h-3.5"></i> Gerar Incentivo da IA
                        </button>
                    </div>

                    <!-- Vendedor 3: Leo -->
                    <div class="glass-card rounded-xl p-4 relative border-t-4 border-t-blue-500">
                        <div class="flex justify-between items-start mb-2">
                            <div>
                                <h4 class="font-bold text-white">Leo</h4>
                                <span class="text-xs text-gray-400">Filial Bahia</span>
                            </div>
                            <span class="text-xs font-bold px-2 py-0.5 rounded bg-blue-500/20 text-blue-400 border border-blue-500/30">
                                85% da Meta
                            </span>
                        </div>
                        <div class="my-3">
                            <div class="flex justify-between text-xs text-gray-400 mb-1">
                                <span>Realizado: R$ 127.500</span>
                                <span>Meta: R$ 150.000</span>
                            </div>
                            <div class="w-full bg-gray-700 h-2 rounded-full overflow-hidden">
                                <div class="bg-blue-500 h-full rounded-full" style="width: 85%"></div>
                            </div>
                        </div>
                        <p class="text-xs text-gray-300 mb-3"><strong>Foco do mês:</strong> Kits de motor MWM e Cummins.</p>
                        <button onclick="gerarIncentivo('Leo', 'Bahia', 85, 'Kits MWM')" class="w-full py-2 px-3 bg-brand-blue hover:bg-blue-600 text-white rounded-lg text-xs font-semibold flex items-center justify-center gap-1.5 transition">
                            <i data-lucide="sparkles" class="w-3.5 h-3.5"></i> Gerar Incentivo da IA
                        </button>
                    </div>

                </div>

                <!-- BOX DE RESPOSTA DA IA SIMULADA -->
                <div id="ai-incentive-box" class="bg-gray-900/90 rounded-xl p-4 border border-brand-accent/40 hidden">
                    <div class="flex items-center gap-2 mb-2">
                        <i data-lucide="bot" class="text-brand-accent w-5 h-5"></i>
                        <h4 id="incentive-title" class="font-bold text-brand-accent text-sm">Orientação da IA para Fabiano (Gestor)</h4>
                    </div>
                    <p id="incentive-text" class="text-sm text-gray-200 italic leading-relaxed"></p>
                    <div class="mt-3 flex justify-end">
                        <button onclick="copiarTextoIncentivo()" class="text-xs bg-gray-800 hover:bg-gray-700 text-gray-300 px-3 py-1 rounded border border-gray-600 flex items-center gap-1">
                            <i data-lucide="copy" class="w-3 h-3"></i> Copiar Roteiro de Fala
                        </button>
                    </div>
                </div>
            </div>

            <!-- SLIDE 3: ASSISTENTE DE WHATSAPP E E-MAIL -->
            <div id="slide-3" class="slide-container flex-col py-4">
                <div class="flex flex-col md:flex-row justify-between items-start md:items-center mb-6 gap-2">
                    <div>
                        <span class="text-xs font-bold text-brand-accent tracking-widest uppercase tech-font">Solução #2</span>
                        <h2 class="text-2xl md:text-3xl font-bold text-white">Assistente de WhatsApp & E-mail Comercial</h2>
                    </div>
                    <span class="text-xs bg-green-900/40 text-green-300 px-3 py-1 rounded-full border border-green-700/50 flex items-center gap-1">
                        <i data-lucide="message-square" class="w-3.5 h-3.5"></i> Automação de Atendimento
                    </span>
                </div>

                <p class="text-gray-300 text-sm md:text-base mb-6">
                    Mecânicos e produtores rurais costumam mandar áudios longos e mensagens confusas. A IA lê/ouve, extrai a lista de peças e gera o rascunho da resposta pronta para seu pai ou vendedores enviarem!
                </p>

                <!-- SIMULADOR DE MENSAGEM DO CLIENTE -->
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-4">
                    
                    <!-- Lado Esquerdo: Entrada do Cliente -->
                    <div class="bg-gray-900/90 rounded-xl p-4 border border-gray-700">
                        <div class="flex items-center justify-between pb-3 mb-3 border-b border-gray-800">
                            <div class="flex items-center gap-2">
                                <div class="w-8 h-8 rounded-full bg-green-600 flex items-center justify-center font-bold text-white text-xs">
                                    M
                                </div>
                                <div>
                                    <h4 class="text-sm font-bold text-white">Oficina Dozel Diesel (Seu João)</h4>
                                    <span class="text-xs text-gray-400">Mensagem via WhatsApp</span>
                                </div>
                            </div>
                            <span class="text-xs text-gray-500">14:32</span>
                        </div>
                        
                        <!-- Conteúdo da mensagem simulada -->
                        <div class="bg-gray-800/90 p-3 rounded-lg text-xs text-gray-300 leading-relaxed mb-4 border-l-2 border-green-500">
                            <p class="font-medium text-green-400 mb-1">🎤 [Áudio de 2 min 45 seg transcrito pela IA]:</p>
                            "Fala Fabiano, tudo bão? Cara, tô com um trator John Deere 6110J parado aqui na oficina de Uberlândia. Preciso com urgência do jogo de bronzinas de biela, os anéis de segmento e a junta do cabeçote do motor PowerTech 4.5L. Vê se você tem na filial de Uberlândia ou se precisa mandar de BH. Me passa o preço total e o prazo de entrega!"
                        </div>

                        <button onclick="processarMensagemWhatsApp()" id="btn-processar-wa" class="w-full py-2.5 bg-green-600 hover:bg-green-500 text-white font-bold rounded-lg text-xs flex items-center justify-center gap-2 transition shadow-md">
                            <i data-lucide="bot" class="w-4 h-4"></i> Processar com IA da Bodipasa
                        </button>
                    </div>

                    <!-- Lado Direito: Saída Inteligente da IA -->
                    <div class="glass-card rounded-xl p-4 border border-blue-500/30 flex flex-col justify-between">
                        <div>
                            <div class="flex items-center gap-2 pb-3 mb-3 border-b border-gray-800">
                                <i data-lucide="cpu" class="text-brand-blue w-5 h-5"></i>
                                <h4 class="text-sm font-bold text-white">Resumo & Orçamento Automático</h4>
                            </div>

                            <div id="wa-result-placeholder" class="py-12 text-center text-gray-500 text-xs">
                                Clique no botão ao lado para ver a IA processando o áudio do cliente...
                            </div>

                            <div id="wa-result-content" class="hidden space-y-3">
                                <div class="bg-gray-900/80 p-2.5 rounded border border-gray-700/60 text-xs">
                                    <p class="text-gray-400 font-semibold mb-1">📋 Resumo da Solicitação:</p>
                                    <ul class="list-disc list-inside text-gray-300 space-y-0.5">
                                        <li>Veículo: Trator John Deere 6110J (Motor PowerTech 4.5L)</li>
                                        <li>Peças: Jogo Bronzinas, Anéis Segmento, Junta Cabeçote.</li>
                                        <li>Local de entrega: Oficina em Uberlândia.</li>
                                    </ul>
                                </div>

                                <div class="bg-blue-950/40 p-2.5 rounded border border-blue-800/60 text-xs text-blue-200">
                                    <p class="font-bold text-blue-400 mb-1">💬 Sugestão de Resposta para enviar no Zap:</p>
                                    <p class="italic">"Olá Seu João! Temos todas as peças em estoque na filial de Uberlândia para o PowerTech 4.5L. Total: R$ 1.890,00. Retirada imediata ou entregamos em até 2h. Posso fechar o pedido?"</p>
                                </div>
                            </div>
                        </div>

                        <div id="wa-actions" class="hidden pt-3 border-t border-gray-800 flex gap-2">
                            <button onclick="alert('Rascunho copiado! Pronto para colar no WhatsApp do cliente.')" class="w-full py-2 bg-gray-800 hover:bg-gray-700 text-white rounded text-xs font-semibold flex items-center justify-center gap-1">
                                <i data-lucide="copy" class="w-3.5 h-3.5"></i> Copiar Resposta
                            </button>
                        </div>
                    </div>

                </div>
            </div>

            <!-- SLIDE 4: CONTROLE DE ESTOQUE DIESEL -->
            <div id="slide-4" class="slide-container flex-col py-4">
                <div class="flex flex-col md:flex-row justify-between items-start md:items-center mb-6 gap-2">
                    <div>
                        <span class="text-xs font-bold text-brand-accent tracking-widest uppercase tech-font">Solução #3</span>
                        <h2 class="text-2xl md:text-3xl font-bold text-white">Controle Inteligente de Estoque entre Filiais</h2>
                    </div>
                    <span class="text-xs bg-amber-900/40 text-amber-300 px-3 py-1 rounded-full border border-amber-700/50">
                        Integração BH • Uberlândia • Bahia
                    </span>
                </div>

                <p class="text-gray-300 text-sm md:text-base mb-6">
                    A IA monitora o giro de peças de alta demanda da Bodipasa e avisa seu pai sobre o estoque crítico antes que a venda seja perdida, sugerindo transferências rápidas!
                </p>

                <!-- TABELA INTERATIVA DE ESTOQUE -->
                <div class="glass-card rounded-xl overflow-hidden mb-4 border border-gray-700">
                    <div class="overflow-x-auto">
                        <table class="w-full text-left text-xs text-gray-300">
                            <thead class="bg-gray-900/90 text-gray-400 uppercase tech-font font-bold">
                                <tr>
                                    <th class="p-3">Código / Peça Diesel</th>
                                    <th class="p-3">Belo Horizonte</th>
                                    <th class="p-3">Uberlândia</th>
                                    <th class="p-3">Bahia</th>
                                    <th class="p-3 text-center">Status IA</th>
                                    <th class="p-3 text-right">Ação Sugerida</th>
                                </tr>
                            </thead>
                            <tbody class="divide-y divide-gray-800">
                                <tr class="hover:bg-gray-800/50">
                                    <td class="p-3 font-semibold text-white">
                                        Piston MWM 229 6-Cilindros<br>
                                        <span class="text-[10px] text-gray-500">SKU: MWM-9821</span>
                                    </td>
                                    <td class="p-3 text-green-400 font-bold">18 un.</td>
                                    <td class="p-3 text-red-400 font-bold">2 un. ⚠️</td>
                                    <td class="p-3 text-green-400 font-bold">12 un.</td>
                                    <td class="p-3 text-center">
                                        <span class="px-2 py-0.5 rounded bg-red-900/50 text-red-300 border border-red-700/50 font-semibold">Crítico em UDI</span>
                                    </td>
                                    <td class="p-3 text-right">
                                        <button onclick="simularTransferencia('Piston MWM 229', 'BH', 'Uberlândia', 5)" class="px-2.5 py-1 bg-brand-accent hover:bg-amber-600 text-black font-bold rounded text-[11px] transition">
                                            Transferir BH ➔ UDI
                                        </button>
                                    </td>
                                </tr>

                                <tr class="hover:bg-gray-800/50">
                                    <td class="p-3 font-semibold text-white">
                                        Kits Bicos Injetores Bosch Cummins 6CT<br>
                                        <span class="text-[10px] text-gray-500">SKU: BSC-6CT-09</span>
                                    </td>
                                    <td class="p-3 text-amber-400 font-bold">4 un.</td>
                                    <td class="p-3 text-green-400 font-bold">15 un.</td>
                                    <td class="p-3 text-red-400 font-bold">1 un. ⚠️</td>
                                    <td class="p-3 text-center">
                                        <span class="px-2 py-0.5 rounded bg-red-900/50 text-red-300 border border-red-700/50 font-semibold">Crítico na Bahia</span>
                                    </td>
                                    <td class="p-3 text-right">
                                        <button onclick="simularTransferencia('Bicos Injetores Bosch', 'Uberlândia', 'Bahia', 4)" class="px-2.5 py-1 bg-brand-accent hover:bg-amber-600 text-black font-bold rounded text-[11px] transition">
                                            Transferir UDI ➔ BA
                                        </button>
                                    </td>
                                </tr>

                                <tr class="hover:bg-gray-800/50">
                                    <td class="p-3 font-semibold text-white">
                                        Turbina Master Power Scania 113<br>
                                        <span class="text-[10px] text-gray-500">SKU: MP-SC113</span>
                                    </td>
                                    <td class="p-3 text-green-400 font-bold">8 un.</td>
                                    <td class="p-3 text-green-400 font-bold">6 un.</td>
                                    <td class="p-3 text-green-400 font-bold">7 un.</td>
                                    <td class="p-3 text-center">
                                        <span class="px-2 py-0.5 rounded bg-green-900/50 text-green-300 border border-green-700/50 font-semibold">Normal</span>
                                    </td>
                                    <td class="p-3 text-right">
                                        <span class="text-gray-500 text-[11px]">Estoque Ok</span>
                                    </td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>

                <!-- NOTIFICAÇÃO DE TRANSFERÊNCIA SIMULADA -->
                <div id="stock-alert-box" class="bg-blue-950/80 border border-blue-500/50 rounded-xl p-3 flex items-center justify-between hidden">
                    <div class="flex items-center gap-2">
                        <i data-lucide="truck" class="text-brand-accent w-5 h-5"></i>
                        <span id="stock-alert-text" class="text-xs text-gray-200"></span>
                    </div>
                    <span class="text-[10px] bg-green-500 text-black font-bold px-2 py-0.5 rounded">Ordem de Remanejamento Gerada</span>
                </div>
            </div>

            <!-- SLIDE 5: CARTÃO DIGITAL INTERATIVO -->
            <div id="slide-5" class="slide-container flex-col py-4">
                <div class="flex flex-col md:flex-row justify-between items-start md:items-center mb-6 gap-2">
                    <div>
                        <span class="text-xs font-bold text-brand-accent tracking-widest uppercase tech-font">Solução #4</span>
                        <h2 class="text-2xl md:text-3xl font-bold text-white">Cartão de Visita Digital Interativo</h2>
                    </div>
                    <span class="text-xs bg-purple-900/40 text-purple-300 px-3 py-1 rounded-full border border-purple-700/50">
                        Ferramenta de Vendas Direta
                    </span>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-2 gap-6 items-center">
                    <div>
                        <p class="text-gray-300 text-sm md:text-base mb-4">
                            Em vez de cartões de papel que o cliente perde, cada vendedor (e o próprio Fabiano) terá um <strong>Cartão Digital Interativo</strong> para enviar no WhatsApp dos mecânicos e frotistas.
                        </p>
                        
                        <ul class="space-y-2.5 text-xs text-gray-300 mb-6">
                            <li class="flex items-center gap-2">
                                <i data-lucide="check-circle-2" class="text-brand-accent w-4 h-4"></i>
                                Botão direto para abrir conversa no WhatsApp.
                            </li>
                            <li class="flex items-center gap-2">
                                <i data-lucide="check-circle-2" class="text-brand-accent w-4 h-4"></i>
                                Catálogo rápido de peças diesel mais vendidas.
                            </li>
                            <li class="flex items-center gap-2">
                                <i data-lucide="check-circle-2" class="text-brand-accent w-4 h-4"></i>
                                Localização GPS das filiais (BH, Uberlândia, Bahia).
                            </li>
                        </ul>

                        <div class="p-3 bg-gray-900/80 rounded-lg border border-gray-800 text-xs text-gray-400">
                            💡 <strong>Dica de Impacto:</strong> Ao final de cada orçamento, o vendedor envia este link. O cliente salva no celular e lembra da Bodipasa na próxima urgência!
                        </div>
                    </div>

                    <!-- PREVIEW DO CARTÃO DIGITAL -->
                    <div class="flex justify-center">
                        <div class="w-full max-w-sm glass-card rounded-2xl p-5 border border-brand-accent/30 shadow-2xl relative overflow-hidden bg-gradient-to-b from-gray-800 to-gray-900">
                            <div class="text-center mb-4">
                                <div class="w-16 h-16 bg-gradient-to-tr from-brand-accent to-amber-600 rounded-full mx-auto flex items-center justify-center text-black font-black text-xl tech-font shadow-lg mb-2">
                                    B
                                </div>
                                <h3 class="text-lg font-bold text-white">FABIANO</h3>
                                <p class="text-xs text-brand-accent font-semibold">Diretor Operacional & Vendas</p>
                                <p class="text-[11px] text-gray-400 mt-0.5">Bodipasa - Peças Diesel e Agrícola</p>
                            </div>

                            <div class="space-y-2 mb-4">
                                <a href="#" onclick="alert('Simulação: Abrindo WhatsApp da Bodipasa...')" class="w-full py-2.5 bg-green-600 hover:bg-green-500 text-white rounded-lg text-xs font-bold flex items-center justify-center gap-2 transition">
                                    <i data-lucide="message-circle" class="w-4 h-4"></i> Solicitar Peça pelo WhatsApp
                                </a>
                                <a href="#" onclick="alert('Simulação: Abrindo Catálogo Diesel em PDF/Web...')" class="w-full py-2 bg-gray-700 hover:bg-gray-600 text-gray-200 rounded-lg text-xs font-semibold flex items-center justify-center gap-2 transition">
                                    <i data-lucide="book-open" class="w-4 h-4"></i> Ver Catálogo de Motores
                                </a>
                            </div>

                            <div class="pt-3 border-t border-gray-700/80">
                                <p class="text-[10px] text-gray-400 text-center mb-2">Nossas Unidades:</p>
                                <div class="flex justify-around text-[10px] text-gray-300 font-medium">
                                    <span class="bg-gray-800 px-2 py-1 rounded">📍 BH</span>
                                    <span class="bg-gray-800 px-2 py-1 rounded">📍 Uberlândia</span>
                                    <span class="bg-gray-800 px-2 py-1 rounded">📍 Bahia</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- SLIDE 6: PLANO DE AÇÃO E CONVITE -->
            <div id="slide-6" class="slide-container flex-col items-center justify-center text-center py-6">
                <div class="w-16 h-16 bg-gradient-to-tr from-brand-accent to-amber-500 rounded-2xl flex items-center justify-center mb-4 text-black shadow-lg">
                    <i data-lucide="rocket" class="w-8 h-8"></i>
                </div>

                <h2 class="text-2xl md:text-4xl font-extrabold text-white mb-3 tech-font">
                    Pronto para dar esse passo na <span class="text-brand-accent">Bodipasa</span>?
                </h2>

                <p class="text-gray-300 text-sm md:text-base max-w-xl mb-6 leading-relaxed">
                    Não precisamos mudar tudo de uma vez. Podemos começar testando um <strong>Painel Simples de Metas</strong> ou a <strong>IA para o WhatsApp</strong> durante 1 semana!
                </p>

                <div class="glass-card rounded-2xl p-6 text-left max-w-2xl w-full mb-8 border-l-4 border-l-green-500 space-y-3">
                    <h4 class="text-sm font-bold text-white flex items-center gap-2">
                        <i data-lucide="check-circle-2" class="text-green-400"></i> O que ganha a Bodipasa com isso?
                    </h4>
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-3 text-xs text-gray-300">
                        <div class="bg-gray-800/60 p-2.5 rounded">
                            ✨ <strong>Zero perda de tempo:</strong> Cálculos e resumos feitos instantaneamente.
                        </div>
                        <div class="bg-gray-800/60 p-2.5 rounded">
                            ✨ <strong>Equipe Motivada:</strong> Incentivos diários para Wesley, Dafine e Leo.
                        </div>
                        <div class="bg-gray-800/60 p-2.5 rounded">
                            ✨ <strong>Estoque Afiado:</strong> Menos peças paradas e mais integração entre filiais.
                        </div>
                        <div class="bg-gray-800/60 p-2.5 rounded">
                            ✨ <strong>Atendimento Rápido:</strong> Orçamentos de motores sem fila no WhatsApp.
                        </div>
                    </div>
                </div>

                <button onclick="finalizarApresentacao()" class="px-8 py-3.5 bg-gradient-to-r from-brand-accent to-amber-600 hover:from-amber-500 hover:to-amber-700 text-black font-extrabold rounded-xl text-base tech-font tracking-wide flex items-center gap-2 shadow-xl transition transform hover:scale-105">
                    <i data-lucide="thumbs-up" class="w-5 h-5"></i> VAMOS FAZER UM TESTE PRÁTICO!
                </button>
            </div>

        </div>
    </main>

    <!-- FOOTER COM CONTROLES DOS SLIDES -->
    <footer class="w-full border-t border-gray-800 bg-brand-dark/90 backdrop-blur-md px-4 py-3 sticky bottom-0 z-50">
        <div class="max-w-5xl mx-auto flex justify-between items-center">
            
            <button id="btn-prev" onclick="mudarSlide(-1)" class="px-4 py-2 bg-gray-800 hover:bg-gray-700 text-gray-300 rounded-lg font-medium text-xs md:text-sm flex items-center gap-1.5 transition disabled:opacity-30 disabled:cursor-not-allowed">
                <i data-lucide="chevron-left" class="w-4 h-4"></i> Voltar
            </button>

            <div class="flex items-center gap-1.5">
                <span id="slide-indicator" class="text-xs font-bold text-gray-400 tech-font">
                    Slide <span text-brand-accent class="text-brand-accent">1</span> de 6
                </span>
            </div>

            <button id="btn-next" onclick="mudarSlide(1)" class="px-5 py-2 bg-brand-accent hover:bg-amber-600 text-black font-bold rounded-lg text-xs md:text-sm flex items-center gap-1.5 transition shadow-lg">
                Próximo <i data-lucide="chevron-right" class="w-4 h-4"></i>
            </button>
        </div>
    </footer>

    <!-- LOGICA JAVASCRIPT DOS SLIDES E INTERAÇÕES -->
    <script>
        let slideAtual = 1;
        const totalSlides = 6;

        // Inicializar Lucide Icons
        lucide.createIcons();

        function atualizarNavegacao() {
            // Esconder todos os slides
            for (let i = 1; i <= totalSlides; i++) {
                const el = document.getElementById(`slide-${i}`);
                if (el) el.classList.remove('active');
            }

            // Mostrar slide atual
            const slideAtivo = document.getElementById(`slide-${slideAtual}`);
            if (slideAtivo) slideAtivo.classList.add('active');

            // Atualizar barra de progresso
            const progressBar = document.getElementById('progress-bar');
            progressBar.style.width = `${(slideAtual / totalSlides) * 100}%`;

            // Atualizar texto do indicador
            const indicator = document.getElementById('slide-indicator');
            indicator.innerHTML = `Slide <span class="text-brand-accent">${slideAtual}</span> de ${totalSlides}`;

            // Controlar estado dos botões
            document.getElementById('btn-prev').disabled = (slideAtual === 1);
            
            const btnNext = document.getElementById('btn-next');
            if (slideAtual === totalSlides) {
                btnNext.style.display = 'none';
            } else {
                btnNext.style.display = 'flex';
            }

            // Re-inicializar ícones para novos elementos visíveis
            lucide.createIcons();
        }

        function mudarSlide(direcao) {
            slideAtual += direcao;
            if (slideAtual < 1) slideAtual = 1;
            if (slideAtual > totalSlides) slideAtual = totalSlides;
            atualizarNavegacao();
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        // --- SIMULAÇÃO SLIDE 2: GERADOR DE INCENTIVOS DA IA ---
        function gerarIncentivo(nome, filial, metaPercent, produtoFoco) {
            const box = document.getElementById('ai-incentive-box');
            const title = document.getElementById('incentive-title');
            const text = document.getElementById('incentive-text');

            title.innerText = `💡 Roteiro de Incentivo da IA para Fabiano aplicar com ${nome} (${filial})`;
            
            let mensagem = "";
            if (metaPercent >= 90) {
                mensagem = `"Fabiano, o ${nome} está voando em ${filial} com ${metaPercent}% da meta batida! Sugiro enviar esta mensagem no privado: 'Fala ${nome}, excelente trabalho na venda de ${produtoFoco} este mês! Falta muito pouco pra estourar a meta. Se bater 100% até sexta, o almoço de sexta é por minha conta! Parabéns pelo empenho!'"`;
            } else if (metaPercent >= 80) {
                mensagem = `"Fabiano, o ${nome} está em um ritmo bom na Bahia (${metaPercent}%). Abordagem sugerida: 'Fala ${nome}! Vi que você já atingiu ${metaPercent}% focando em ${produtoFoco}. Temos mais 5 dias úteis. Se a gente focar nos clientes frotistas antigos essa semana, você fecha o mês com chave de ouro! Conta comigo se precisar de desconto em algum lote.'"`;
            } else {
                mensagem = `"Fabiano, a ${nome} está com ${metaPercent}% da meta em Uberlândia. Em vez de cobrar de forma dura, use esta abordagem encorajadora: 'Oi ${nome}, vi que a linha de ${produtoFoco} deu uma desacelerada essa semana. Quer que eu veja se conseguimos puxar algumas unidades da filial de BH com preço especial pra você fechar com aqueles 2 clientes pendentes?'"`;
            }

            text.innerText = mensagem;
            box.classList.remove('hidden');
            box.scrollIntoView({ behavior: 'smooth', block: 'nearest' });
        }

        function copiarTextoIncentivo() {
            const texto = document.getElementById('incentive-text').innerText;
            const element = document.createElement('textarea');
            element.value = texto;
            document.body.appendChild(element);
            element.select();
            document.execCommand('copy');
            document.body.removeChild(element);
            alert('Roteiro copiado com sucesso! Você pode colar no WhatsApp do funcionário.');
        }

        // --- SIMULAÇÃO SLIDE 3: PROCESSAR WHATSAPP DE CLIENTE DIESEL ---
        function processarMensagemWhatsApp() {
            const btn = document.getElementById('btn-processar-wa');
            const placeholder = document.getElementById('wa-result-placeholder');
            const content = document.getElementById('wa-result-content');
            const actions = document.getElementById('wa-actions');

            btn.innerHTML = `<i data-lucide="loader-2" class="w-4 h-4 animate-spin"></i> Transcrevendo & Consultando Estoque...`;
            lucide.createIcons();

            setTimeout(() => {
                placeholder.classList.add('hidden');
                content.classList.remove('hidden');
                actions.classList.remove('hidden');
                btn.innerHTML = `<i data-lucide="check" class="w-4 h-4"></i> Áudio Analisado com Sucesso!`;
                btn.classList.remove('bg-green-600', 'hover:bg-green-500');
                btn.classList.add('bg-gray-700');
                lucide.createIcons();
            }, 1200);
        }

        // --- SIMULAÇÃO SLIDE 4: TRANSFERÊNCIA DE ESTOQUE ---
        function simularTransferencia(peca, origem, destino, qtd) {
            const box = document.getElementById('stock-alert-box');
            const text = document.getElementById('stock-alert-text');

            text.innerHTML = `Solicitada a transferência de <strong>${qtd} unidades</strong> de <em>${peca}</em> da filial <strong>${origem}</strong> para a filial <strong>${destino}</strong>. Notificação enviada ao depósito!`;
            box.classList.remove('hidden');
            box.scrollIntoView({ behavior: 'smooth', block: 'nearest' });
        }

        // --- SIMULAÇÃO SLIDE 6: CONCLUSÃO ---
        function finalizarApresentacao() {
            alert('Excelente, Fabiano! O próximo passo é definir qual dessas automações você quer testar primeiro na Bodipasa nesta semana!');
        }

        // Suporte para navegação pelas setas do teclado
        document.addEventListener('keydown', function(e) {
            if (e.key === 'ArrowRight') {
                mudarSlide(1);
            } else if (e.key === 'ArrowLeft') {
                mudarSlide(-1);
            }
        });
    </script>
</body>
</html>
