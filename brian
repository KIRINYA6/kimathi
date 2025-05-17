<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Brian Kirinya | Community Case Manager</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        .editable {
            border: 1px dashed transparent;
            padding: 2px;
            transition: all 0.3s;
        }
        .editable:hover {
            border-color: #3b82f6;
            background-color: rgba(59, 130, 246, 0.05);
        }
        .edit-mode .editable {
            border-color: #3b82f6;
            background-color: rgba(59, 130, 246, 0.05);
        }
        #editPanel {
            transition: transform 0.3s ease;
        }
        .hidden {
            transform: translateX(100%);
        }
    </style>
</head>
<body class="font-sans bg-gray-50">
    <!-- Edit Panel -->
    <div id="editPanel" class="fixed top-0 right-0 h-full w-64 bg-white shadow-lg z-50 p-4 overflow-y-auto hidden">
        <div class="flex justify-between items-center mb-4">
            <h3 class="text-lg font-bold">Edit Mode</h3>
            <button id="closeEditPanel" class="text-gray-500 hover:text-gray-700">
                <i class="fas fa-times"></i>
            </button>
        </div>
        <div class="space-y-4">
            <div>
                <label class="block text-sm font-medium text-gray-700 mb-1">Name</label>
                <input id="editName" type="text" class="w-full p-2 border rounded">
            </div>
            <div>
                <label class="block text-sm font-medium text-gray-700 mb-1">Title</label>
                <input id="editTitle" type="text" class="w-full p-2 border rounded">
            </div>
            <div>
                <label class="block text-sm font-medium text-gray-700 mb-1">Organization</label>
                <input id="editOrg" type="text" class="w-full p-2 border rounded">
            </div>
            <div>
                <label class="block text-sm font-medium text-gray-700 mb-1">About Text</label>
                <textarea id="editAbout" class="w-full p-2 border rounded h-24"></textarea>
            </div>
            <div>
                <label class="block text-sm font-medium text-gray-700 mb-1">Services</label>
                <textarea id="editServices" class="w-full p-2 border rounded h-24"></textarea>
            </div>
            <div>
                <label class="block text-sm font-medium text-gray-700 mb-1">Contact Email</label>
                <input id="editEmail" type="text" class="w-full p-2 border rounded">
            </div>
            <div>
                <label class="block text-sm font-medium text-gray-700 mb-1">Phone</label>
                <input id="editPhone" type="text" class="w-full p-2 border rounded">
            </div>
            <button id="saveChanges" class="w-full bg-blue-600 text-white py-2 rounded hover:bg-blue-700 transition">
                Save Changes
            </button>
            <div class="text-xs text-gray-500 mt-4">
                Changes are saved to your browser's local storage.
            </div>
        </div>
    </div>

    <!-- Edit Button -->
    <button id="editButton" class="fixed bottom-4 right-4 bg-blue-600 text-white p-3 rounded-full shadow-lg z-40 hover:bg-blue-700 transition">
        <i class="fas fa-edit"></i>
    </button>

    <!-- Main Content -->
    <div class="container mx-auto px-4 py-8">
        <!-- Header -->
        <header class="flex flex-col md:flex-row items-center justify-between mb-12">
            <div class="flex items-center mb-6 md:mb-0">
                <div class="w-16 h-16 rounded-full bg-blue-100 flex items-center justify-center mr-4">
                    <i class="fas fa-user text-blue-600 text-2xl"></i>
                </div>
                <div>
                    <h1 id="name" class="editable text-2xl font-bold text-gray-800">Brian Kirinya</h1>
                    <p id="title" class="editable text-blue-600">Community Case Manager</p>
                    <p id="org" class="editable text-gray-600">KeyCare Hub</p>
                </div>
            </div>
            <nav class="flex space-x-4">
                <a href="#about" class="px-3 py-2 text-gray-700 hover:text-blue-600 transition">About</a>
                <a href="#services" class="px-3 py-2 text-gray-700 hover:text-blue-600 transition">Services</a>
                <a href="#contact" class="px-3 py-2 text-gray-700 hover:text-blue-600 transition">Contact</a>
            </nav>
        </header>

        <!-- Hero Section -->
        <section class="bg-gradient-to-r from-blue-50 to-indigo-50 rounded-xl p-8 mb-12">
            <div class="max-w-3xl mx-auto text-center">
                <h2 class="text-3xl font-bold text-gray-800 mb-4">Supporting Community Health and Wellbeing</h2>
                <p class="text-lg text-gray-600 mb-6">Dedicated to providing compassionate case management services to enhance quality of life and access to care.</p>
                <a href="#contact" class="inline-block bg-blue-600 text-white px-6 py-3 rounded-lg hover:bg-blue-700 transition">
                    Get in Touch <i class="fas fa-arrow-right ml-2"></i>
                </a>
            </div>
        </section>

        <!-- About Section -->
        <section id="about" class="mb-16">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-8 md:mb-0 md:pr-8">
                    <img src="https://images.unsplash.com/photo-1579684385127-1ef15d508118?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=880&q=80" 
                         alt="Community support" 
                         class="rounded-xl shadow-lg w-full h-auto">
                </div>
                <div class="md:w-1/2">
                    <h2 class="text-2xl font-bold text-gray-800 mb-4">About Me</h2>
                    <div id="aboutText" class="editable text-gray-600 space-y-4">
                        <p>As a dedicated Community Case Manager at KeyCare Hub, I bring over 8 years of experience in coordinating care and support services for individuals and families in need. My approach is client-centered, focusing on empowering individuals to achieve their highest level of independence and wellbeing.</p>
                        <p>I specialize in connecting clients with appropriate community resources, advocating for their needs, and developing comprehensive care plans that address both immediate concerns and long-term goals.</p>
                        <p>My work is guided by principles of compassion, respect, and cultural sensitivity, ensuring that every client receives personalized support tailored to their unique circumstances.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Services Section -->
        <section id="services" class="mb-16 bg-gray-50 rounded-xl p-8">
            <h2 class="text-2xl font-bold text-gray-800 mb-8 text-center">My Services</h2>
            <div id="servicesContent" class="editable grid md:grid-cols-3 gap-6">
                <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-lg transition">
                    <div class="text-blue-600 mb-4">
                        <i class="fas fa-hands-helping text-3xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Care Coordination</h3>
                    <p class="text-gray-600">Comprehensive assessment and coordination of medical, social, and community services to ensure seamless care delivery.</p>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-lg transition">
                    <div class="text-blue-600 mb-4">
                        <i class="fas fa-users text-3xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Community Resource Linking</h3>
                    <p class="text-gray-600">Connecting clients with appropriate local resources including housing, food assistance, and mental health services.</p>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-lg transition">
                    <div class="text-blue-600 mb-4">
                        <i class="fas fa-user-shield text-3xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Advocacy</h3>
                    <p class="text-gray-600">Representing client needs and rights within healthcare systems and community organizations to ensure access to quality care.</p>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-lg transition">
                    <div class="text-blue-600 mb-4">
                        <i class="fas fa-file-medical text-3xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Care Planning</h3>
                    <p class="text-gray-600">Developing individualized care plans that address physical, emotional, and social needs with measurable goals.</p>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-lg transition">
                    <div class="text-blue-600 mb-4">
                        <i class="fas fa-home text-3xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Housing Support</h3>
                    <p class="text-gray-600">Assistance with transitional housing, shelter placement, and permanent housing solutions for vulnerable populations.</p>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-lg transition">
                    <div class="text-blue-600 mb-4">
                        <i class="fas fa-heartbeat text-3xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Health Education</h3>
                    <p class="text-gray-600">Providing education on disease management, medication adherence, and healthy lifestyle choices.</p>
                </div>
            </div>
        </section>

        <!-- Testimonials -->
        <section class="mb-16">
            <h2 class="text-2xl font-bold text-gray-800 mb-8 text-center">Client Testimonials</h2>
            <div class="grid md:grid-cols-2 gap-6">
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-200 flex items-center justify-center mr-4">
                            <i class="fas fa-user text-gray-500"></i>
                        </div>
                        <div>
                            <h4 class="font-bold">Sarah M.</h4>
                            <p class="text-sm text-gray-500">Client since 2021</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic">"Brian helped navigate the complex healthcare system when I was at my most vulnerable. His persistence and compassion made all the difference in getting me the care I needed."</p>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-200 flex items-center justify-center mr-4">
                            <i class="fas fa-user text-gray-500"></i>
                        </div>
                        <div>
                            <h4 class="font-bold">James T.</h4>
                            <p class="text-sm text-gray-500">Client since 2022</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic">"Thanks to Brian's advocacy, my father finally received the home care services he needed. He treated us like family and went above and beyond to ensure we understood all our options."</p>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="bg-blue-600 text-white rounded-xl p-8 mb-12">
            <div class="max-w-4xl mx-auto">
                <h2 class="text-2xl font-bold mb-6">Contact Me</h2>
                <div class="grid md:grid-cols-2 gap-8">
                    <div>
                        <h3 class="text-xl font-semibold mb-4">Get in Touch</h3>
                        <div class="space-y-4">
                            <div class="flex items-start">
                                <i class="fas fa-envelope mt-1 mr-4"></i>
                                <div>
                                    <p class="font-medium">Email</p>
                                    <p id="email" class="editable">brian.kirinya@keycarehub.org</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <i class="fas fa-phone mt-1 mr-4"></i>
                                <div>
                                    <p class="font-medium">Phone</p>
                                    <p id="phone" class="editable">(555) 123-4567</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <i class="fas fa-map-marker-alt mt-1 mr-4"></i>
                                <div>
                                    <p class="font-medium">Location</p>
                                    <p>KeyCare Hub, 123 Wellness Ave, Suite 200<br>Cityville, ST 12345</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div>
                        <h3 class="text-xl font-semibold mb-4">Send a Message</h3>
                        <form class="space-y-4">
                            <div>
                                <label for="contactName" class="block mb-1">Your Name</label>
                                <input type="text" id="contactName" class="w-full p-2 rounded text-gray-800">
                            </div>
                            <div>
                                <label for="contactEmail" class="block mb-1">Your Email</label>
                                <input type="email" id="contactEmail" class="w-full p-2 rounded text-gray-800">
                            </div>
                            <div>
                                <label for="contactMessage" class="block mb-1">Message</label>
                                <textarea id="contactMessage" rows="4" class="w-full p-2 rounded text-gray-800"></textarea>
                            </div>
                            <button type="submit" class="bg-white text-blue-600 px-6 py-2 rounded-lg hover:bg-gray-100 transition">
                                Send Message <i class="fas fa-paper-plane ml-2"></i>
                            </button>
                        </form>
                    </div>
                </div>
            </div>
        </section>

        <!-- Footer -->
        <footer class="border-t border-gray-200 pt-8 pb-6">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-4 md:mb-0">
                    <p class="text-gray-600">&copy; <span id="currentYear"></span> Brian Kirinya. All rights reserved.</p>
                </div>
                <div class="flex space-x-4">
                    <a href="#" class="text-gray-600 hover:text-blue-600 transition">
                        <i class="fab fa-linkedin text-xl"></i>
                    </a>
                    <a href="#" class="text-gray-600 hover:text-blue-600 transition">
                        <i class="fab fa-twitter text-xl"></i>
                    </a>
                    <a href="#" class="text-gray-600 hover:text-blue-600 transition">
                        <i class="fab fa-facebook text-xl"></i>
                    </a>
                </div>
            </div>
        </footer>
    </div>

    <script>
        // Set current year
        document.getElementById('currentYear').textContent = new Date().getFullYear();

        // Edit Mode Functionality
        const editButton = document.getElementById('editButton');
        const editPanel = document.getElementById('editPanel');
        const closeEditPanel = document.getElementById('closeEditPanel');
        const saveChanges = document.getElementById('saveChanges');
        
        // Form fields
        const editName = document.getElementById('editName');
        const editTitle = document.getElementById('editTitle');
        const editOrg = document.getElementById('editOrg');
        const editAbout = document.getElementById('editAbout');
        const editServices = document.getElementById('editServices');
        const editEmail = document.getElementById('editEmail');
        const editPhone = document.getElementById('editPhone');
        
        // Content elements
        const nameEl = document.getElementById('name');
        const titleEl = document.getElementById('title');
        const orgEl = document.getElementById('org');
        const aboutTextEl = document.getElementById('aboutText');
        const servicesContentEl = document.getElementById('servicesContent');
        const emailEl = document.getElementById('email');
        const phoneEl = document.getElementById('phone');

        // Toggle edit panel
        editButton.addEventListener('click', () => {
            editPanel.classList.toggle('hidden');
            document.body.classList.toggle('edit-mode');
            
            // Populate form fields with current content
            editName.value = nameEl.textContent;
            editTitle.value = titleEl.textContent;
            editOrg.value = orgEl.textContent;
            editAbout.value = aboutTextEl.innerHTML.replace(/<br>/g, '\n').replace(/<\/p><p>/g, '\n\n');
            editServices.value = servicesContentEl.innerHTML;
            editEmail.value = emailEl.textContent;
            editPhone.value = phoneEl.textContent;
        });

        closeEditPanel.addEventListener('click', () => {
            editPanel.classList.add('hidden');
            document.body.classList.remove('edit-mode');
        });

        // Save changes
        saveChanges.addEventListener('click', () => {
            // Update content with form values
            nameEl.textContent = editName.value;
            titleEl.textContent = editTitle.value;
            orgEl.textContent = editOrg.value;
            
            // Convert newlines to paragraphs for about text
            const aboutText = editAbout.value.split('\n\n').map(para => `<p>${para.replace(/\n/g, '<br>')}</p>`).join('');
            aboutTextEl.innerHTML = aboutText;
            
            emailEl.textContent = editEmail.value;
            phoneEl.textContent = editPhone.value;
            
            // Save to localStorage
            localStorage.setItem('profileName', editName.value);
            localStorage.setItem('profileTitle', editTitle.value);
            localStorage.setItem('profileOrg', editOrg.value);
            localStorage.setItem('profileAbout', editAbout.value);
            localStorage.setItem('profileServices', editServices.value);
            localStorage.setItem('profileEmail', editEmail.value);
            localStorage.setItem('profilePhone', editPhone.value);
            
            // Close panel
            editPanel.classList.add('hidden');
            document.body.classList.remove('edit-mode');
            
            alert('Changes saved!');
        });

        // Load saved content
        function loadSavedContent() {
            if (localStorage.getItem('profileName')) {
                nameEl.textContent = localStorage.getItem('profileName');
                titleEl.textContent = localStorage.getItem('profileTitle');
                orgEl.textContent = localStorage.getItem('profileOrg');
                
                const savedAbout = localStorage.getItem('profileAbout');
                if (savedAbout) {
                    const aboutText = savedAbout.split('\n\n').map(para => `<p>${para.replace(/\n/g, '<br>')}</p>`).join('');
                    aboutTextEl.innerHTML = aboutText;
                }
                
                emailEl.textContent = localStorage.getItem('profileEmail');
                phoneEl.textContent = localStorage.getItem('profilePhone');
            }
        }

        // Initialize
        loadSavedContent();

        // Simple form submission (demo only)
        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your message! This is a demo - no message was actually sent.');
            this.reset();
        });
    </script>
</body>
</html>
