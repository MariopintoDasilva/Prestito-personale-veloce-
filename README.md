<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Credito Personale Rapido - Da Silva Alcide Mario Pinto</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#5D5CDE',
                        'primary-dark': '#4A4AC8'
                    }
                }
            }
        }
    </script>
    <style>
        .gradient-bg {
            background: linear-gradient(135deg, #5D5CDE 0%, #4A4AC8 100%);
        }
        .floating-animation {
            animation: float 3s ease-in-out infinite;
        }
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }
        .success-modal {
            backdrop-filter: blur(10px);
        }
    </style>
</head>
<body class="bg-white dark:bg-gray-900 transition-colors duration-300">

    <!-- Header -->
    <header class="gradient-bg shadow-lg">
        <div class="container mx-auto px-4 py-6">
            <div class="flex items-center justify-between">
                <div class="text-white">
                    <h1 class="text-2xl md:text-3xl font-bold">Credito Personale Rapido</h1>
                    <p class="text-blue-100">Da Silva Alcide Mario Pinto</p>
                </div>
                <div class="text-white text-right">
                    <div class="flex items-center space-x-2">
                        <i class="fas fa-percentage"></i>
                        <span class="text-xl font-bold">2% Tasso</span>
                    </div>
                    <p class="text-sm text-blue-100">Interesse Annuale</p>
                </div>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="py-16 bg-gradient-to-br from-blue-50 to-indigo-100 dark:from-gray-800 dark:to-gray-900">
        <div class="container mx-auto px-4 text-center">
            <div class="floating-animation">
                <h2 class="text-4xl md:text-6xl font-bold text-gray-800 dark:text-white mb-6">
                    Prestiti Fino a <span class="text-primary">500.000€</span>
                </h2>
                <p class="text-xl text-gray-600 dark:text-gray-300 mb-8 max-w-3xl mx-auto">
                    Ottieni il tuo prestito personale con il miglior tasso di interesse del 2%. 
                    Processo rapido, sicuro e completamente online.
                </p>
            </div>
            <div class="grid md:grid-cols-3 gap-8 mt-12">
                <div class="bg-white dark:bg-gray-800 p-6 rounded-xl shadow-lg">
                    <i class="fas fa-clock text-primary text-3xl mb-4"></i>
                    <h3 class="text-xl font-bold text-gray-800 dark:text-white mb-2">Approvazione Rapida</h3>
                    <p class="text-gray-600 dark:text-gray-300">Risposta entro 24 ore</p>
                </div>
                <div class="bg-white dark:bg-gray-800 p-6 rounded-xl shadow-lg">
                    <i class="fas fa-shield-alt text-primary text-3xl mb-4"></i>
                    <h3 class="text-xl font-bold text-gray-800 dark:text-white mb-2">100% Sicuro</h3>
                    <p class="text-gray-600 dark:text-gray-300">Dati protetti e crittografati</p>
                </div>
                <div class="bg-white dark:bg-gray-800 p-6 rounded-xl shadow-lg">
                    <i class="fas fa-euro-sign text-primary text-3xl mb-4"></i>
                    <h3 class="text-xl font-bold text-gray-800 dark:text-white mb-2">Tasso Vantaggioso</h3>
                    <p class="text-gray-600 dark:text-gray-300">Solo 2% di interesse annuale</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Loan Calculator -->
    <section class="py-16 bg-white dark:bg-gray-900">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center text-gray-800 dark:text-white mb-12">Calcolatore Prestito</h2>
            <div class="max-w-2xl mx-auto bg-gray-50 dark:bg-gray-800 p-8 rounded-xl shadow-lg">
                <div class="space-y-6">
                    <div>
                        <label class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                            Importo del Prestito (€)
                        </label>
                        <input type="range" id="loanAmount" min="1000" max="500000" value="50000" step="1000"
                               class="w-full h-2 bg-gray-200 rounded-lg appearance-none cursor-pointer dark:bg-gray-700">
                        <div class="flex justify-between text-sm text-gray-500 dark:text-gray-400 mt-1">
                            <span>1.000€</span>
                            <span id="amountDisplay" class="font-bold text-primary">50.000€</span>
                            <span>500.000€</span>
                        </div>
                    </div>
                    
                    <div>
                        <label class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                            Durata (mesi)
                        </label>
                        <input type="range" id="loanDuration" min="12" max="120" value="36" step="6"
                               class="w-full h-2 bg-gray-200 rounded-lg appearance-none cursor-pointer dark:bg-gray-700">
                        <div class="flex justify-between text-sm text-gray-500 dark:text-gray-400 mt-1">
                            <span>12 mesi</span>
                            <span id="durationDisplay" class="font-bold text-primary">36 mesi</span>
                            <span>120 mesi</span>
                        </div>
                    </div>
                    
                    <div class="bg-primary text-white p-4 rounded-lg text-center">
                        <p class="text-sm mb-2">Rata Mensile Stimata</p>
                        <p id="monthlyPayment" class="text-2xl font-bold">€1.451</p>
                        <p class="text-sm mt-2 opacity-90">Tasso di interesse: 2% annuale</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Application Form -->
    <section class="py-16 bg-gradient-to-br from-gray-50 to-blue-50 dark:from-gray-800 dark:to-gray-900">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center text-gray-800 dark:text-white mb-4">Richiedi il Tuo Prestito</h2>
            <p class="text-center text-gray-600 dark:text-gray-300 mb-12">Compila il modulo e riceverai una risposta immediata</p>
            
            <div class="max-w-3xl mx-auto">
                <form id="loanForm" class="bg-white dark:bg-gray-800 p-8 rounded-xl shadow-lg space-y-6">
                    <div class="grid md:grid-cols-2 gap-6">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">Nome*</label>
                            <input type="text" id="firstName" required
                                   class="w-full px-4 py-3 text-base border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-700 dark:border-gray-600 dark:text-white">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">Cognome*</label>
                            <input type="text" id="lastName" required
                                   class="w-full px-4 py-3 text-base border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-700 dark:border-gray-600 dark:text-white">
                        </div>
                    </div>

                    <div class="grid md:grid-cols-2 gap-6">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">Email*</label>
                            <input type="email" id="email" required
                                   class="w-full px-4 py-3 text-base border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-700 dark:border-gray-600 dark:text-white">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">Telefono*</label>
                            <input type="tel" id="phone" required
                                   class="w-full px-4 py-3 text-base border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-700 dark:border-gray-600 dark:text-white">
                        </div>
                    </div>

                    <div class="grid md:grid-cols-2 gap-6">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">Importo Richiesto (€)*</label>
                            <input type="number" id="requestedAmount" min="1000" max="500000" required
                                   class="w-full px-4 py-3 text-base border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-700 dark:border-gray-600 dark:text-white">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">Reddito Mensile (€)*</label>
                            <input type="number" id="monthlyIncome" required
                                   class="w-full px-4 py-3 text-base border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-700 dark:border-gray-600 dark:text-white">
                        </div>
                    </div>

                    <div>
                        <label class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">Motivo del Prestito</label>
                        <select id="loanPurpose"
                                class="w-full px-4 py-3 text-base border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-700 dark:border-gray-600 dark:text-white">
                            <option value="">Seleziona un motivo</option>
                            <option value="casa">Acquisto/Ristrutturazione Casa</option>
                            <option value="auto">Acquisto Automobile</option>
                            <option value="consolidamento">Consolidamento Debiti</option>
                            <option value="business">Avvio/Espansione Business</option>
                            <option value="emergenza">Spese di Emergenza</option>
                            <option value="altro">Altro</option>
                        </select>
                    </div>

                    <div>
                        <label class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">Note Aggiuntive</label>
                        <textarea id="additionalNotes" rows="4"
                                  class="w-full px-4 py-3 text-base border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-700 dark:border-gray-600 dark:text-white"
                                  placeholder="Informazioni aggiuntive..."></textarea>
                    </div>

                    <div class="flex items-start space-x-3">
                        <input type="checkbox" id="terms" required
                               class="mt-1 w-4 h-4 text-primary bg-gray-100 border-gray-300 rounded focus:ring-primary dark:focus:ring-primary-dark dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600">
                        <label for="terms" class="text-sm text-gray-700 dark:text-gray-300">
                            Accetto i <a href="#" class="text-primary hover:underline">termini e condizioni</a> 
                            e l'<a href="#" class="text-primary hover:underline">informativa sulla privacy</a>*
                        </label>
                    </div>

                    <button type="submit" 
                            class="w-full bg-primary hover:bg-primary-dark text-white font-bold py-4 px-6 rounded-lg transition-colors duration-300 text-lg">
                        <i class="fas fa-paper-plane mr-2"></i>
                        Invia Richiesta Prestito
                    </button>
                </form>
            </div>
        </div>
    </section>

    <!-- WhatsApp Contact -->
    <section class="py-16 bg-primary">
        <div class="container mx-auto px-4 text-center">
            <div class="max-w-2xl mx-auto">
                <h2 class="text-3xl font-bold text-white mb-6">Hai Domande?</h2>
                <p class="text-blue-100 mb-8 text-lg">Contattaci direttamente su WhatsApp per un supporto immediato</p>
                <a href="https://wa.me/message/IBU2WZ7O6M72C1" target="_blank"
                   class="inline-flex items-center bg-green-500 hover:bg-green-600 text-white font-bold py-4 px-8 rounded-lg transition-colors duration-300 text-lg">
                    <i class="fab fa-whatsapp text-2xl mr-3"></i>
                    Chatta con Noi su WhatsApp
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-12">
        <div class="container mx-auto px-4">
            <div class="grid md:grid-cols-3 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4">Credito Personale Rapido</h3>
                    <p class="text-gray-300 mb-4">Da Silva Alcide Mario Pinto</p>
                    <p class="text-gray-400">Prestiti sicuri e convenienti con il miglior tasso di interesse del mercato.</p>
                </div>
                <div>
                    <h4 class="text-lg font-semibold mb-4">Contatti</h4>
                    <div class="space-y-2">
                        <p class="text-gray-300">
                            <i class="fas fa-envelope mr-2"></i>
                            josepintodasilva32@gmail.com
                        </p>
                        <a href="https://wa.me/message/IBU2WZ7O6M72C1" class="text-green-400 hover:text-green-300">
                            <i class="fab fa-whatsapp mr-2"></i>
                            WhatsApp Support
                        </a>
                    </div>
                </div>
                <div>
                    <h4 class="text-lg font-semibold mb-4">Informazioni</h4>
                    <ul class="space-y-2 text-gray-300">
                        <li>Tasso di Interesse: 2% annuale</li>
                        <li>Importo Max: €500.000</li>
                        <li>Approvazione: 24 ore</li>
                        <li>100% Sicuro e Garantito</li>
                    </ul>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-8 pt-8 text-center text-gray-400">
                <p>&copy; 2025 Da Silva Alcide Mario Pinto. Tutti i diritti riservati.</p>
            </div>
        </div>
    </footer>

    <!-- Success Modal -->
    <div id="successModal" class="fixed inset-0 bg-black bg-opacity-50 success-modal hidden items-center justify-center z-50">
        <div class="bg-white dark:bg-gray-800 p-8 rounded-xl shadow-2xl max-w-md w-full mx-4 text-center">
            <div class="text-green-500 text-6xl mb-4">
                <i class="fas fa-check-circle"></i>
            </div>
            <h3 class="text-2xl font-bold text-gray-800 dark:text-white mb-4">Richiesta Inviata!</h3>
            <p class="text-gray-600 dark:text-gray-300 mb-6">
                La tua richiesta di prestito è stata inviata con successo. 
                Riceverai una risposta entro 24 ore.
            </p>
            <button onclick="closeModal()" 
                    class="bg-primary hover:bg-primary-dark text-white font-bold py-3 px-6 rounded-lg transition-colors duration-300">
                Chiudi
            </button>
        </div>
    </div>

    <script>
        // Dark mode detection
        if (window.matchMedia && window.matchMedia('(prefers-color-scheme: dark)').matches) {
            document.documentElement.classList.add('dark');
        }
        window.matchMedia('(prefers-color-scheme: dark)').addEventListener('change', event => {
            if (event.matches) {
                document.documentElement.classList.add('dark');
            } else {
                document.documentElement.classList.remove('dark');
            }
        });

        // Loan Calculator
        const loanAmount = document.getElementById('loanAmount');
        const loanDuration = document.getElementById('loanDuration');
        const amountDisplay = document.getElementById('amountDisplay');
        const durationDisplay = document.getElementById('durationDisplay');
        const monthlyPayment = document.getElementById('monthlyPayment');

        function calculatePayment() {
            const principal = parseFloat(loanAmount.value);
            const duration = parseInt(loanDuration.value);
            const annualRate = 0.02; // 2%
            const monthlyRate = annualRate / 12;
            
            const payment = (principal * monthlyRate * Math.pow(1 + monthlyRate, duration)) / 
                           (Math.pow(1 + monthlyRate, duration) - 1);
            
            amountDisplay.textContent = principal.toLocaleString('it-IT') + '€';
            durationDisplay.textContent = duration + ' mesi';
            monthlyPayment.textContent = '€' + Math.round(payment).toLocaleString('it-IT');
        }

        loanAmount.addEventListener('input', calculatePayment);
        loanDuration.addEventListener('input', calculatePayment);
        calculatePayment(); // Initial calculation

        // Form submission
        document.getElementById('loanForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const formData = {
                firstName: document.getElementById('firstName').value,
                lastName: document.getElementById('lastName').value,
                email: document.getElementById('email').value,
                phone: document.getElementById('phone').value,
                requestedAmount: document.getElementById('requestedAmount').value,
                monthlyIncome: document.getElementById('monthlyIncome').value,
                loanPurpose: document.getElementById('loanPurpose').value || 'Non specificato',
                additionalNotes: document.getElementById('additionalNotes').value || 'Nessuna'
            };

            // Create WhatsApp message
            const whatsappMessage = `🏦 *NUOVA RICHIESTA PRESTITO*
            
👤 *Cliente:* ${formData.firstName} ${formData.lastName}
📧 *Email:* ${formData.email}
📱 *Telefono:* ${formData.phone}
💰 *Importo Richiesto:* €${parseInt(formData.requestedAmount).toLocaleString('it-IT')}
💵 *Reddito Mensile:* €${parseInt(formData.monthlyIncome).toLocaleString('it-IT')}
🎯 *Motivo:* ${formData.loanPurpose}
📝 *Note:* ${formData.additionalNotes}

---
Inviato da: Credito Personale Rapido
Data: ${new Date().toLocaleString('it-IT')}`;

            // Create email content
            const emailSubject = `Nuova Richiesta Prestito - ${formData.firstName} ${formData.lastName}`;
            const emailBody = `Nome: ${formData.firstName} ${formData.lastName}
Email: ${formData.email}
Telefono: ${formData.phone}
Importo Richiesto: €${parseInt(formDa
