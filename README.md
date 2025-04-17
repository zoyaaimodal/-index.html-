# -index.html-
<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>मेरा ब्लॉग प्लेटफॉर्म</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <link href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        .custom-shadow { box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); }
        .post-card { transition: transform 0.3s ease; }
        .post-card:hover { transform: translateY(-5px); }
        .theme-blue { --primary-color: #3b82f6; }
        .theme-green { --primary-color: #10b981; }
        .theme-purple { --primary-color: #8b5cf6; }
        .theme-red { --primary-color: #ef4444; }
        .theme-active { border: 2px solid #000; }
        .btn-primary { background-color: var(--primary-color, #3b82f6); }
        .text-primary { color: var(--primary-color, #3b82f6); }
        .border-primary { border-color: var(--primary-color, #3b82f6); }
        body { font-family: 'Arial', sans-serif; }
    </style>
</head>
<body class="bg-gray-100 theme-blue">
    <!-- Header -->
    <header class="bg-white shadow-md">
        <div class="container mx-auto px-4 py-3">
            <div class="flex justify-between items-center">
                <div class="flex items-center">
                    <h1 class="text-2xl font-bold text-primary">मेरा ब्लॉग</h1>
                </div>
                <nav class="hidden md:flex space-x-4">
                    <a href="#" class="text-gray-600 hover:text-primary" id="home-link">होम</a>
                    <a href="#" class="text-gray-600 hover:text-primary" id="profile-link">प्रोफाइल</a>
                    <a href="#" class="text-gray-600 hover:text-primary" id="upload-link">अपलोड</a>
                    <a href="#" class="text-gray-600 hover:text-primary" id="customize-link">कस्टमाइज़</a>
                </nav>
                <div class="md:hidden">
                    <button id="mobile-menu-button" class="text-gray-500 hover:text-primary">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
            <!-- Mobile Menu -->
            <div id="mobile-menu" class="md:hidden hidden mt-2 space-y-2">
                <a href="#" class="block py-2 text-gray-600 hover:text-primary" id="home-link-mobile">होम</a>
                <a href="#" class="block py-2 text-gray-600 hover:text-primary" id="profile-link-mobile">प्रोफाइल</a>
                <a href="#" class="block py-2 text-gray-600 hover:text-primary" id="upload-link-mobile">अपलोड</a>
                <a href="#" class="block py-2 text-gray-600 hover:text-primary" id="customize-link-mobile">कस्टमाइज़</a>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <main class="container mx-auto px-4 py-6">
        <!-- Home Section -->
        <section id="home-section" class="mb-8">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                <!-- Main Content Area -->
                <div class="md:col-span-2">
                    <h2 class="text-2xl font-bold mb-4">लेटेस्ट पोस्ट</h2>
                    
                    <!-- Posts -->
                    <div class="space-y-6">
                        <!-- Post 1 -->
                        <div class="bg-white rounded-lg shadow-md p-4 post-card">
                            <div class="flex items-center mb-3">
                                <img src="https://cdn.jsdelivr.net/gh/shivammadaan/dummy-images/profile/profile1.jpg" alt="User" class="w-10 h-10 rounded-full mr-3">
                                <div>
                                    <h3 class="font-bold">राहुल शर्मा</h3>
                                    <p class="text-sm text-gray-500">2 घंटे पहले</p>
                                </div>
                            </div>
                            <p class="mb-3">नई दिल्ली का मेरा सफर! बहुत ही अच्छा अनुभव रहा। आप सभी को भी एक बार जरूर जाना चाहिए।</p>
                            <div class="mb-3">
                                <img src="https://cdn.jsdelivr.net/gh/shivammadaan/dummy-images/delhi/india-gate.jpg" alt="Delhi Trip" class="w-full rounded-lg">
                            </div>
                            <div class="flex justify-between text-sm">
                                <button class="flex items-center text-gray-600 hover:text-blue-500"><i class="far fa-thumbs-up mr-1"></i> <span class="like-count">24</span> लाइक</button>
                                <button class="flex items-center text-gray-600 hover:text-green-500"><i class="far fa-comment mr-1"></i> <span>8</span> कमेंट</button>
                                <button class="flex items-center text-gray-600 hover:text-red-500"><i class="far fa-share-square mr-1"></i> शेयर</button>
                            </div>
                        </div>
                        
                        <!-- Post 2 -->
                        <div class="bg-white rounded-lg shadow-md p-4 post-card">
                            <div class="flex items-center mb-3">
                                <img src="https://cdn.jsdelivr.net/gh/shivammadaan/dummy-images/profile/profile2.jpg" alt="User" class="w-10 h-10 rounded-full mr-3">
                                <div>
                                    <h3 class="font-bold">प्रिया वर्मा</h3>
                                    <p class="text-sm text-gray-500">5 घंटे पहले</p>
                                </div>
                            </div>
                            <p class="mb-3">मेरा नया कुकिंग वीडियो! आज हम बनाएंगे स्पेशल पनीर बटर मसाला।</p>
                            <div class="mb-3 relative" style="padding-top: 56.25%;">
                                <video class="absolute top-0 left-0 w-full h-full rounded-lg" controls playsinline webkit-playsinline>
                                    <source src="https://cdn.jsdelivr.net/gh/shivammadaan/dummy-videos/cooking.mp4" type="video/mp4">
                                    आपका ब्राउज़र वीडियो का समर्थन नहीं करता है।
                                </video>
                            </div>
                            <div class="flex justify-between text-sm">
                                <button class="flex items-center text-gray-600 hover:text-blue-500"><i class="far fa-thumbs-up mr-1"></i> <span class="like-count">42</span> लाइक</button>
                                <button class="flex items-center text-gray-600 hover:text-green-500"><i class="far fa-comment mr-1"></i> <span>15</span> कमेंट</button>
                                <button class="flex items-center text-gray-600 hover:text-red-500"><i class="far fa-share-square mr-1"></i> शेयर</button>
                            </div>
                        </div>
                        
                        <!-- Post 3 -->
                        <div class="bg-white rounded-lg shadow-md p-4 post-card">
                            <div class="flex items-center mb-3">
                                <img src="https://cdn.jsdelivr.net/gh/shivammadaan/dummy-images/profile/profile3.jpg" alt="User" class="w-10 h-10 rounded-full mr-3">
                                <div>
                                    <h3 class="font-bold">अमित पटेल</h3>
                                    <p class="text-sm text-gray-500">1 दिन पहले</p>
                                </div>
                            </div>
                            <p class="mb-3">आज का मौसम बहुत सुहावना है। मैंने कुछ तस्वीरें खींची हैं, आशा है आपको पसंद आएंगी।</p>
                            <div class="grid grid-cols-2 gap-2 mb-3">
                                <img src="https://cdn.jsdelivr.net/gh/shivammadaan/dummy-images/nature/nature1.jpg" alt="Nature" class="w-full rounded-lg">
                                <img src="https://cdn.jsdelivr.net/gh/shivammadaan/dummy-images/nature/nature2.jpg" alt="Nature" class="w-full rounded-lg">
                                <img src="https://cdn.jsdelivr.net/gh/shivammadaan/dummy-images/nature/nature3.jpg" alt="Nature" class="w-full rounded-lg">
                                <img src="https://cdn.jsdelivr.net/gh/shivammadaan/dummy-images/nature/nature4.jpg" alt="Nature" class="w-full rounded-lg">
                            </div>
                            <div class="flex justify-between text-sm">
                                <button class="flex items-center text-gray-600 hover:text-blue-500"><i class="far fa-thumbs-up mr-1"></i> <span class="like-count">18</span> लाइक</button>
                                <button class="flex items-center text-gray-600 hover:text-green-500"><i class="far fa-comment mr-1"></i> <span>5</span> कमेंट</button>
                                <button class="flex items-center text-gray-600 hover:text-red-500"><i class="far fa-share-square mr-1"></i> शेयर</button>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Sidebar -->
                <div class="md:col-span-1">
                    <!-- Profile Card -->
                    <div class="bg-white rounded-lg shadow-md p-4 mb-4">
                        <div class="flex flex-col items-center">
                            <img src="https://cdn.jsdelivr.net/gh/shivammadaan/dummy-images/profile/user-avatar.jpg" alt="Profile" class="w-20 h-20 rounded-full mb-3">
                            <h3 class="font-bold text-lg">अपना नाम</h3>
                            <p class="text-gray-500 mb-3">@username</p>
                            <div class="flex space-x-4 mb-3">
                                <div class="text-center">
                                    <p class="font-bold">42</p>
                                    <p class="text-sm text-gray-500">पोस्ट</p>
                                </div>
                                <div class="text-center">
                                    <p class="font-bold">156</p>
                                    <p class="text-sm text-gray-500">फॉलोअर्स</p>
                                </div>
                                <div class="text-center">
                                    <p class="font-bold">128</p>
                                    <p class="text-sm text-gray-500">फॉलोइंग</p>
                                </div>
                            </div>
                            <button class="w-full py-2 btn-primary text-white rounded-lg">प्रोफाइल एडिट करें</button>
                        </div>
                    </div>
                    
                    <!-- Advertisement -->
                    <div class="bg-white rounded-lg shadow-md p-4 mb-4">
                        <h3 class="font-bold text-gray-500 mb-2 text-center text-sm">विज्ञापन</h3>
                        <div class="bg-gray-200 h-48 flex items-center justify-center rounded">
                            <p class="text-gray-500">यहां आपका विज्ञापन होगा</p>
                        </div>
                    </div>
                    
                    <!-- Trending Topics -->
                    <div class="bg-white rounded-lg shadow-md p-4">
                        <h3 class="font-bold mb-3">ट्रेंडिंग टॉपिक्स</h3>
                        <ul class="space-y-2">
                            <li><a href="#" class="text-primary hover:underline">#फेस्टिवल2023</a></li>
                            <li><a href="#" class="text-primary hover:underline">#ट्रैवल</a></li>
                            <li><a href="#" class="text-primary hover:underline">#न्यूटेक</a></li>
                            <li><a href="#" class="text-primary hover:underline">#फूड</a></li>
                            <li><a href="#" class="text-primary hover:underline">#फिटनेस</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <!-- Upload Section -->
        <section id="upload-section" class="mb-8 hidden">
            <div class="bg-white rounded-lg shadow-md p-6">
                <h2 class="text-2xl font-bold mb-4">नया कंटेंट अपलोड करें</h2>
                
                <div class="mb-4">
                    <label class="block text-gray-700 mb-2">पोस्ट टाइटल</label>
                    <input type="text" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-primary" placeholder="एक टाइटल दें...">
                </div>
                
                <div class="mb-4">
                    <label class="block text-gray-700 mb-2">पोस्ट कंटेंट</label>
                    <textarea class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-primary" rows="4" placeholder="अपनी बात लिखें..."></textarea>
                </div>
                
                <div class="mb-6">
                    <h3 class="text-lg font-semibold mb-3">मीडिया अपलोड करें</h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <!-- Photo Upload -->
                        <div class="border-2 border-dashed border-gray-300 rounded-lg p-4 text-center cursor-pointer hover:bg-gray-50" id="photo-upload">
                            <i class="fas fa-image text-4xl text-gray-400 mb-2"></i>
                            <p class="text-gray-500">फोटो अपलोड करें</p>
                            <p class="text-sm text-gray-400">JPG, PNG (अधिकतम 5MB)</p>
                            <input type="file" accept="image/*" class="hidden" id="photo-input">
                        </div>
                        
                        <!-- Video Upload -->
                        <div class="border-2 border-dashed border-gray-300 rounded-lg p-4 text-center cursor-pointer hover:bg-gray-50" id="video-upload">
                            <i class="fas fa-video text-4xl text-gray-400 mb-2"></i>
                            <p class="text-gray-500">वीडियो अपलोड करें</p>
                            <p class="text-sm text-gray-400">MP4, MOV (अधिकतम 50MB)</p>
                            <input type="file" accept="video/*" class="hidden" id="video-input">
                        </div>
                    </div>
                </div>
                
                <div class="flex justify-between">
                    <button class="px-6 py-2 bg-gray-300 text-gray-700 rounded-lg hover:bg-gray-400">रद्द करें</button>
                    <button class="px-6 py-2 btn-primary text-white rounded-lg hover:bg-blue-600">पोस्ट करें</button>
                </div>
            </div>
            
            <!-- Preview Section -->
            <div class="mt-6 hidden" id="preview-section">
                <h3 class="text-xl font-bold mb-3">प्रीव्यू</h3>
                <div class="bg-white rounded-lg shadow-md p-4">
                    <div id="preview-content" class="mb-4"></div>
                </div>
            </div>
        </section>

        <!-- Profile Section -->
        <section id="profile-section" class="mb-8 hidden">
            <div class="bg-white rounded-lg shadow-md p-6">
                <div class="flex flex-col md:flex-row">
                    <div class="md:w-1/3 flex flex-col items-center mb-6 md:mb-0">
                        <img src="https://cdn.jsdelivr.net/gh/shivammadaan/dummy-images/profile/user-avatar.jpg" alt="Profile" class="w-32 h-32 rounded-full mb-4">
                        <button class="px-4 py-2 text-sm text-primary border border-primary rounded-lg">प्रोफाइल फोटो बदलें</button>
                    </div>
                    <div class="md:w-2/3">
                        <h2 class="text-2xl font-bold mb-4">प्रोफाइल सेटिंग्स</h2>
                        
                        <div class="mb-4">
                            <label class="block text-gray-700 mb-2">यूज़रनेम</label>
                            <input type="text" value="@username" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-primary">
                        </div>
                        
                        <div class="mb-4">
                            <label class="block text-gray-700 mb-2">नाम</label>
                            <input type="text" value="अपना नाम" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-primary">
                        </div>
                        
                        <div class="mb-4">
                            <label class="block text-gray-700 mb-2">बायो</label>
                            <textarea class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-primary" rows="3">यहां अपने बारे में लिखें...</textarea>
                        </div>
                        
                        <div class="mb-4">
                            <label class="block text-gray-700 mb-2">ईमेल</label>
                            <input type="email" value="example@email.com" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-primary">
                        </div>
                        
                        <div class="mb-4">
                            <label class="block text-gray-700 mb-2">मोबाइल नंबर</label>
                            <input type="tel" value="+91 9876543210" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-primary">
                        </div>
                        
                        <div class="text-right">
                            <button class="px-6 py-2 btn-primary text-white rounded-lg hover:bg-blue-600">सेव करें</button>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Social Media Links -->
            <div class="mt-6 bg-white rounded-lg shadow-md p-6">
                <h3 class="text-xl font-bold mb-4">सोशल मीडिया लिंक्स</h3>
                
                <div class="space-y-4">
                    <div class="flex items-center">
                        <i class="fab fa-youtube text-red-600 text-2xl w-10"></i>
                        <input type="text" placeholder="YouTube चैनल URL" class="flex-1 ml-2 px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-primary">
                    </div>
                    
                    <div class="flex items-center">
                        <i class="fab fa-facebook text-blue-600 text-2xl w-10"></i>
                        <input type="text" placeholder="Facebook पेज URL" class="flex-1 ml-2 px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-primary">
                    </div>
                    
                    <div class="flex items-center">
                        <i class="fab fa-instagram text-pink-600 text-2xl w-10"></i>
                        <input type="text" placeholder="Instagram प्रोफाइल URL" class="flex-1 ml-2 px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-primary">
                    </div>
                    
                    <div class="flex items-center">
                        <i class="fab fa-twitter text-blue-400 text-2xl w-10"></i>
                        <input type="text" placeholder="Twitter प्रोफाइल URL" class="flex-1 ml-2 px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-primary">
                    </div>
                </div>
                
                <div class="mt-4 text-right">
                    <button class="px-6 py-2 btn-primary text-white rounded-lg hover:bg-blue-600">सेव करें</button>
                </div>
            </div>
        </section>

        <!-- Customize Section -->
        <section id="customize-section" class="mb-8 hidden">
            <div class="bg-white rounded-lg shadow-md p-6">
                <h2 class="text-2xl font-bold mb-4">ब्लॉग कस्टमाइज़ करें</h2>
                
                <!-- Theme Selection -->
                <div class="mb-6">
                    <h3 class="text-lg font-semibold mb-3">थीम चुनें</h3>
                    <div class="flex space-x-4">
                        <div class="theme-option theme-blue theme-active w-10 h-10 rounded-full bg-blue-500 cursor-pointer"></div>
                        <div class="theme-option theme-green w-10 h-10 rounded-full bg-green-500 cursor-pointer"></div>
                        <div class="theme-option theme-purple w-10 h-10 rounded-full bg-purple-500 cursor-pointer"></div>
                        <div class="theme-option theme-red w-10 h-10 rounded-full bg-red-500 cursor-pointer"></div>
                    </div>
                </div>
                
                <!-- Layout Options -->
                <div class="mb-6">
                    <h3 class="text-lg font-semibold mb-3">लेआउट ऑप्शन्स</h3>
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                        <div class="layout-option border rounded-lg p-3 cursor-pointer hover:border-primary">
                            <div class="bg-gray-200 h-32 mb-2 rounded flex flex-col">
                                <div class="bg-gray-300 h-6 m-2 rounded"></div>
                                <div class="flex-1 m-2 grid grid-cols-2 gap-2">
                                    <div class="bg-gray-300 rounded"></div>
                                    <div class="bg-gray-300 rounded"></div>
                                </div>
                            </div>
                            <p class="text-center">ग्रिड लेआउट</p>
                        </div>
                        
                        <div class="layout-option border rounded-lg p-3 cursor-pointer hover:border-primary">
                            <div class="bg-gray-200 h-32 mb-2 rounded flex flex-col">
                                <div class="bg-gray-300 h-6 m-2 rounded"></div>
                                <div class="flex-1 m-2">
                                    <div class="bg-gray-300 h-full rounded"></div>
                                </div>
                            </div>
                            <p class="text-center">सिंगल कॉलम</p>
                        </div>
                        
                        <div class="layout-option border rounded-lg p-3 cursor-pointer hover:border-primary">
                            <div class="bg-gray-200 h-32 mb-2 rounded flex flex-col">
                                <div class="bg-gray-300 h-6 m-2 rounded"></div>
                                <div class="flex-1 m-2 flex">
                                    <div class="w-2/3 bg-gray-300 rounded mr-2"></div>
                                    <div class="w-1/3 bg-gray-300 rounded"></div>
                                </div>
                            </div>
                            <p class="text-center">साइडबार के साथ</p>
                        </div>
                    </div>
                </div>
                
                <!-- Advertisement Settings -->
                <div class="mb-6">
                    <h3 class="text-lg font-semibold mb-3">विज्ञापन सेटिंग्स</h3>
                    
                    <div class="mb-4">
                        <label class="block text-gray-700 mb-2">AdSense कोड</label>
                        <textarea class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-primary" rows="3" placeholder="अपना AdSense कोड यहां पेस्ट करें..."></textarea>
                    </div>
                    
                    <div class="mb-4">
                        <label class="flex items-center">
                            <input type="checkbox" class="form-checkbox text-primary h-5 w-5">
                            <span class="ml-2">साइडबार में विज्ञापन दिखाएं</span>
                        </label>
                    </div>
                    
                    <div class="mb-4">
                        <label class="flex items-center">
                            <input type="checkbox" class="form-checkbox text-primary h-5 w-5">
                            <span class="ml-2">पोस्ट के बीच में विज्ञापन दिखाएं</span>
                        </label>
                    </div>
                    
                    <div class="mb-4">
                        <label class="flex items-center">
                            <input type="checkbox" class="form-checkbox text-primary h-5 w-5">
                            <span class="ml-2">वीडियो के पहले विज्ञापन दिखाएं</span>
                        </label>
                    </div>
                </div>
                
                <!-- Footer Settings -->
                <div class="mb-6">
                    <h3 class="text-lg font-semibold mb-3">फुटर सेटिंग्स</h3>
                    <div class="mb-4">
                        <label class="block text-gray-700 mb-2">फुटर टेक्स्ट</label>
                        <input type="text" value="© 2023 मेरा ब्लॉग - सभी अधिकार सुरक्षित" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-primary">
                    </div>
                </div>
                
                <div class="text-right">
                    <button class="px-6 py-2 btn-primary text-white rounded-lg hover:bg-blue-600">सेटिंग्स सेव करें</button>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-white shadow-md py-6">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-4 md:mb-0">
                    <p class="text-gray-600">© 2023 मेरा ब्लॉग - सभी अधिकार सुरक्षित</p>
                </div>
                <div class="flex space-x-4">
                    <a href="#" class="text-gray-600 hover:text-primary"><i class="fab fa-facebook"></i></a>
                    <a href="#" class="text-gray-600 hover:text-primary"><i class="fab fa-twitter"></i></a>
                    <a href="#" class="text-gray-600 hover:text-primary"><i class="fab fa-instagram"></i></a>
                    <a href="#" class="text-gray-600 hover:text-primary"><i class="fab fa-youtube"></i></a>
                </div>
            </div>
            <div class="mt-4 text-center text-sm text-gray-500">
                <a href="#" class="hover:text-primary">प्राइवेसी पॉलिसी</a> • 
                <a href="#" class="hover:text-primary">टर्म्स ऑफ सर्विस</a> • 
                <a href="#" class="hover:text-primary">हेल्प</a> • 
                <a href="#" class="hover:text-primary">कॉन्टैक्ट</a>
            </div>
        </div>
    </footer>

    <!-- JavaScript -->
    <script>
        // Mobile Menu Toggle
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');
        
        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        
        // Section Navigation
        const sections = {
            'home': document.getElementById('home-section'),
            'upload': document.getElementById('upload-section'),
            'profile': document.getElementById('profile-section'),
            'customize': document.getElementById('customize-section')
        };
        
        function showSection(sectionId) {
            // Hide all sections
            Object.values(sections).forEach(section => {
                section.classList.add('hidden');
            });
            
            // Show the selected section
            sections[sectionId].classList.remove('hidden');
        }
        
        // Desktop Nav Links
        document.getElementById('home-link').addEventListener('click', (e) => {
            e.preventDefault();
            showSection('home');
        });
        
        document.getElementById('upload-link').addEventListener('click', (e) => {
            e.preventDefault();
            showSection('upload');
        });
        
        document.getElementById('profile-link').addEventListener('click', (e) => {
            e.preventDefault();
            showSection('profile');
        });
        
        document.getElementById('customize-link').addEventListener('click', (e) => {
            e.preventDefault();
            showSection('customize');
        });
        
        // Mobile Nav Links
        document.getElementById('home-link-mobile').addEventListener('click', (e) => {
            e.preventDefault();
            showSection('home');
            mobileMenu.classList.add('hidden');
        });
        
        document.getElementById('upload-link-mobile').addEventListener('click', (e) => {
            e.preventDefault();
            showSection('upload');
            mobileMenu.classList.add('hidden');
        });
        
        document.getElementById('profile-link-mobile').addEventListener('click', (e) => {
            e.preventDefault();
            showSection('profile');
            mobileMenu.classList.add('hidden');
        });
        
        document.getElementById('customize-link-mobile').addEventListener('click', (e) => {
            e.preventDefault();
            showSection('customize');
            mobileMenu.classList.add('hidden');
        });
        
        // Like Button Functionality
        const likeButtons = document.querySelectorAll('.fa-thumbs-up');
        likeButtons.forEach(button => {
            button.addEventListener('click', (e) => {
                const likeCountElement = e.target.parentElement.querySelector('.like-count');
                let likeCount = parseInt(likeCountElement.textContent);
                if (e.target.classList.contains('far')) {
                    // Like
                    e.target.classList.remove('far');
                    e.target.classList.add('fas');
                    e.target.parentElement.classList.add('text-blue-500');
                    likeCountElement.textContent = likeCount + 1;
                } else {
                    // Unlike
                    e.target.classList.remove('fas');
                    e.target.classList.add('far');
                    e.target.parentElement.classList.remove('text-blue-500');
                    likeCountElement.textContent = likeCount - 1;
                }
            });
        });
        
        // File Upload Functionality
        const photoUpload = document.getElementById('photo-upload');
        const photoInput = document.getElementById('photo-input');
        const videoUpload = document.getElementById('video-upload');
        const videoInput = document.getElementById('video-input');
        const previewSection = document.getElementById('preview-section');
        const previewContent = document.getElementById('preview-content');
        
        photoUpload.addEventListener('click', () => {
            photoInput.click();
        });
        
        videoUpload.addEventListener('click', () => {
            videoInput.click();
        });
        
        photoInput.addEventListener('change', (e) => {
            const file = e.target.files[0];
            if (file) {
                const reader = new FileReader();
                reader.onload = function(event) {
                    previewSection.classList.remove('hidden');
                    previewContent.innerHTML = `<img src="${event.target.result}" alt="Preview" class="max-w-full h-auto rounded-lg">`;
                };
                reader.readAsDataURL(file);
            }
        });
        
        videoInput.addEventListener('change', (e) => {
            const file = e.target.files[0];
            if (file) {
                const url = URL.createObjectURL(file);
                previewSection.classList.remove('hidden');
                previewContent.innerHTML = `
                    <video controls playsinline webkit-playsinline class="max-w-full h-auto rounded-lg">
                        <source src="${url}" type="${file.type}">
                        आपका ब्राउज़र वीडियो का समर्थन नहीं करता है।
                    </video>
                `;
            }
        });
        
        // Theme Selection
        const themeOptions = document.querySelectorAll('.theme-option');
        const body = document.body;
        
        themeOptions.forEach(option => {
            option.addEventListener('click', () => {
                // Remove active class from all options
                themeOptions.forEach(opt => opt.classList.remove('theme-active'));
                
                // Add active class to selected option
                option.classList.add('theme-active');
                
                // Remove all theme classes from body
                body.classList.remove('theme-blue', 'theme-green', 'theme-purple', 'theme-red');
                
                // Add selected theme class to body
                if (option.classList.contains('theme-blue')) {
                    body.classList.add('theme-blue');
                } else if (option.classList.contains('theme-green')) {
                    body.classList.add('theme-green');
                } else if (option.classList.contains('theme-purple')) {
                    body.classList.add('theme-purple');
                } else if (option.classList.contains('theme-red')) {
                    body.classList.add('theme-red');
                }
            });
        });
    </script>
</body>
</html>

