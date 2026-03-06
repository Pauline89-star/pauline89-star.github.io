# pauline89-star.github.io
<!DOCTYPE html>
<html lang="nl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Communicatie Routekaart - Bureau Burgerberaad</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Bebas Neue -->
    <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap" rel="stylesheet">
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    <style>
        body { font-family: 'Tahoma', Geneva, sans-serif; }
        .font-bebas { font-family: 'Bebas Neue', cursive; }
        .metro-scroll::-webkit-scrollbar { height: 6px; }
        .metro-scroll::-webkit-scrollbar-thumb { background: #cbd5e1; border-radius: 10px; }
        
        /* Tooltip styling */
        .tooltip {
            visibility: hidden;
            opacity: 0;
            transition: opacity 0.2s, transform 0.2s;
            transform: translateY(10px) translateX(-50%);
        }
        .station-container:hover .tooltip {
            visibility: visible;
            opacity: 1;
            transform: translateY(0) translateX(-50%);
        }
    </style>
</head>
<body class="bg-slate-100 p-2 md:p-8">

    <div class="max-w-6xl mx-auto bg-white rounded-3xl shadow-2xl overflow-hidden border border-slate-200">
        
        <!-- Header -->
        <div class="p-8 border-b border-slate-200" style="background-color: #afd7d9;">
            <div class="flex items-center gap-4 mb-2">
                <div class="bg-slate-900/10 p-3 rounded-full shadow-inner text-slate-900">
                    <i data-lucide="train" size="32"></i>
                </div>
                <h1 class="text-4xl md:text-6xl font-normal tracking-wider font-bebas uppercase text-slate-900">Communicatie Routekaart</h1>
            </div>
            <p class="text-slate-800 text-lg md:text-xl font-medium italic">
                Draagt het bij aan het lokaal en nationaal inbedden van zorgvuldige, legitieme en impactvolle, (permanente) burgerberaden?
            </p>
        </div>

        <div class="p-6 md:p-10">
            
            <!-- Legenda & Quotes -->
            <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mb-12">
                <div class="flex flex-col gap-2 p-5 bg-white rounded-xl border-l-8 shadow-sm" style="border-color: #5d8c8e;">
                    <div class="flex items-center gap-2 font-bold uppercase text-xs tracking-widest text-slate-500">
                        <div class="w-3 h-3 rounded-full" style="background-color: #5d8c8e;"></div>
                        Blauwe Lijn: Strategie
                    </div>
                    <p class="text-sm font-medium text-slate-700 italic">"Zonder strategie is distributie slechts lawaai."</p>
                </div>
                
                <div class="flex flex-col gap-2 p-5 bg-white rounded-xl border-l-8 shadow-sm" style="border-color: #ffdd65;">
                    <div class="flex items-center gap-2 font-bold uppercase text-xs tracking-widest text-slate-500">
                        <div class="w-3 h-3 rounded-full" style="background-color: #ffdd65;"></div>
                        Gele Lijn: Creatie
                    </div>
                    <p class="text-sm font-medium text-slate-700 italic">"Goede vormgeving vertelt het verhaal zonder woorden."</p>
                </div>

                <div class="flex flex-col gap-2 p-5 bg-white rounded-xl border-l-8 shadow-sm" style="border-color: #61bf89;">
                    <div class="flex items-center gap-2 font-bold uppercase text-xs tracking-widest text-slate-500">
                        <div class="w-3 h-3 rounded-full" style="background-color: #61bf89;"></div>
                        Groene Lijn: Productie
                    </div>
                    <p class="text-sm font-medium text-slate-700 italic">"Even snel een pdfje rondmailen is paniek voetbal."</p>
                </div>
            </div>

            <!-- Metro Kaart -->
            <div class="relative mb-16 py-10 px-4 overflow-x-auto metro-scroll">
                <div class="min-w-[900px] relative">
                    
                    <!-- Strategie Lijn (Blauw) -->
                    <div class="relative mb-12 flex items-center h-20">
                        <div class="absolute -left-4 w-32 -translate-x-full text-right pr-4 font-bold text-[10px] uppercase tracking-widest opacity-40">Strategie Lijn</div>
                        <div class="absolute left-0 right-0 h-4 rounded-full opacity-20" style="background-color: #5d8c8e;"></div>
                        <div class="absolute left-0 h-4 rounded-full w-full" style="background-color: #5d8c8e;"></div>
                        <div class="relative w-full flex justify-between px-10">
                            <!-- Stations worden hieronder handmatig herhaald voor de HTML versie -->
                            <div class="station-container relative flex flex-col items-center">
                                <div class="w-12 h-12 rounded-full border-4 border-white shadow-lg flex items-center justify-center z-10 text-white" style="background-color: #5d8c8e;"><i data-lucide="lightbulb" size="18"></i></div>
                                <span class="mt-4 font-bold text-[10px] uppercase bg-white px-2 py-1 rounded shadow-sm border border-slate-100">Het Idee</span>
                                <div class="tooltip absolute top-20 left-1/2 w-64 p-4 bg-slate-900 text-white text-xs rounded-xl shadow-2xl z-20 pointer-events-none">
                                    <p class="font-bold mb-1 border-b border-white/20 pb-1 uppercase tracking-wider" style="color: #5d8c8e;">Het Idee</p>
                                    <span>Elke campagne begint met een vonk. Is het haalbaar, zinvol en past het bij onze koers?</span>
                                </div>
                            </div>
                            <!-- Station 2 -->
                            <div class="station-container relative flex flex-col items-center">
                                <div class="w-12 h-12 rounded-full border-4 border-white shadow-lg flex items-center justify-center z-10 text-white" style="background-color: #5d8c8e;"><i data-lucide="user-check" size="18"></i></div>
                                <span class="mt-4 font-bold text-[10px] uppercase bg-white px-2 py-1 rounded shadow-sm border border-slate-100">Besluit</span>
                                <div class="tooltip absolute top-20 left-1/2 w-64 p-4 bg-slate-900 text-white text-xs rounded-xl shadow-2xl z-20 pointer-events-none">
                                    <p class="font-bold mb-1 border-b border-white/20 pb-1 uppercase tracking-wider" style="color: #5d8c8e;">Besluit</p>
                                    <span>Officieel akkoord van directie en één vast aanspreekpunt aanwijzen.</span>
                                </div>
                            </div>
                            <!-- Station 3 -->
                            <div class="station-container relative flex flex-col items-center">
                                <div class="w-12 h-12 rounded-full border-4 border-white shadow-lg flex items-center justify-center z-10 text-white" style="background-color: #5d8c8e;"><i data-lucide="file-text" size="18"></i></div>
                                <span class="mt-4 font-bold text-[10px] uppercase bg-white px-2 py-1 rounded shadow-sm border border-slate-100">De Briefing</span>
                                <div class="tooltip absolute top-20 left-1/2 w-64 p-4 bg-slate-900 text-white text-xs rounded-xl shadow-2xl z-20 pointer-events-none">
                                    <p class="font-bold mb-1 border-b border-white/20 pb-1 uppercase tracking-wider" style="color: #5d8c8e;">De Briefing</p>
                                    <span>Bevat: doelstelling, doelgroep, wie, wat, waar, wanneer en budget.</span>
                                </div>
                            </div>
                            <!-- Station 4 -->
                            <div class="station-container relative flex flex-col items-center">
                                <div class="w-12 h-12 rounded-full border-4 border-white shadow-lg flex items-center justify-center z-10 text-white" style="background-color: #5d8c8e;"><i data-lucide="message-square" size="18"></i></div>
                                <span class="mt-4 font-bold text-[10px] uppercase bg-white px-2 py-1 rounded shadow-sm border border-slate-100">Check</span>
                                <div class="tooltip absolute top-20 left-1/2 w-64 p-4 bg-slate-900 text-white text-xs rounded-xl shadow-2xl z-20 pointer-events-none">
                                    <p class="font-bold mb-1 border-b border-white/20 pb-1 uppercase tracking-wider" style="color: #5d8c8e;">Check</p>
                                    <span>Controleer de briefing met directie. Zonder akkoord geen trein.</span>
                                </div>
                            </div>
                            <!-- Station 5 -->
                            <div class="station-container relative flex flex-col items-center">
                                <div class="w-12 h-12 rounded-full border-4 border-white shadow-lg flex items-center justify-center z-10 text-white" style="background-color: #5d8c8e;"><i data-lucide="calendar-days" size="18"></i></div>
                                <span class="mt-4 font-bold text-[10px] uppercase bg-white px-2 py-1 rounded shadow-sm border border-slate-100">Planning</span>
                                <div class="tooltip absolute top-20 left-1/2 w-64 p-4 bg-slate-900 text-white text-xs rounded-xl shadow-2xl z-20 pointer-events-none">
                                    <p class="font-bold mb-1 border-b border-white/20 pb-1 uppercase tracking-wider" style="color: #5d8c8e;">Planning</p>
                                    <span>Check agenda's en reserveer capaciteit voor de uitvoering.</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Creatie Lijn (Geel) -->
                    <div class="relative mb-12 flex items-center h-20">
                        <div class="absolute -left-4 w-32 -translate-x-full text-right pr-4 font-bold text-[10px] uppercase tracking-widest opacity-40">Creatie Lijn</div>
                        <div class="absolute left-0 right-0 h-4 rounded-full opacity-20" style="background-color: #ffdd65;"></div>
                        <div class="absolute left-0 h-4 rounded-full w-full" style="background-color: #ffdd65;"></div>
                        <div class="relative w-full flex justify-between px-10">
                            <div class="station-container relative flex flex-col items-center">
                                <div class="w-12 h-12 rounded-full border-4 border-white shadow-lg flex items-center justify-center z-10 text-slate-900" style="background-color: #ffdd65;"><i data-lucide="file-text" size="18"></i></div>
                                <span class="mt-4 font-bold text-[10px] uppercase bg-white px-2 py-1 rounded shadow-sm border border-slate-100">Inhoud</span>
                                <div class="tooltip absolute top-20 left-1/2 w-64 p-4 bg-slate-900 text-white text-xs rounded-xl shadow-2xl z-20 pointer-events-none">
                                    <p class="font-bold mb-1 border-b border-white/20 pb-1 uppercase tracking-wider" style="color: #ffdd65;">Inhoud</p>
                                    <span>De projectleider levert feitelijke inhoud aan. Input is geen output!</span>
                                </div>
                            </div>
                            <div class="station-container relative flex flex-col items-center">
                                <div class="w-12 h-12 rounded-full border-4 border-white shadow-lg flex items-center justify-center z-10 text-slate-900" style="background-color: #ffdd65;"><i data-lucide="message-square" size="18"></i></div>
                                <span class="mt-4 font-bold text-[10px] uppercase bg-white px-2 py-1 rounded shadow-sm border border-slate-100">Copywriting</span>
                                <div class="tooltip absolute top-20 left-1/2 w-64 p-4 bg-slate-900 text-white text-xs rounded-xl shadow-2xl z-20 pointer-events-none">
                                    <p class="font-bold mb-1 border-b border-white/20 pb-1 uppercase tracking-wider" style="color: #ffdd65;">Copywriting</p>
                                    <span>Communicatie schrijft de teksten voor alle kanalen.</span>
                                </div>
                            </div>
                            <div class="station-container relative flex flex-col items-center">
                                <div class="w-12 h-12 rounded-full border-4 border-white shadow-lg flex items-center justify-center z-10 text-slate-900" style="background-color: #ffdd65;"><i data-lucide="palette" size="18"></i></div>
                                <span class="mt-4 font-bold text-[10px] uppercase bg-white px-2 py-1 rounded shadow-sm border border-slate-100">Vormgeving</span>
                                <div class="tooltip absolute top-20 left-1/2 w-64 p-4 bg-slate-900 text-white text-xs rounded-xl shadow-2xl z-20 pointer-events-none">
                                    <p class="font-bold mb-1 border-b border-white/20 pb-1 uppercase tracking-wider" style="color: #ffdd65;">Vormgeving</p>
                                    <span>Visuele vertaling. Check maten en formats tijdig bij de vormgever!</span>
                                </div>
                            </div>
                            <div class="station-container relative flex flex-col items-center">
                                <div class="w-12 h-12 rounded-full border-4 border-white shadow-lg flex items-center justify-center z-10 text-slate-900" style="background-color: #ffdd65;"><i data-lucide="check-circle-2" size="18"></i></div>
                                <span class="mt-4 font-bold text-[10px] uppercase bg-white px-2 py-1 rounded shadow-sm border border-slate-100">Eindcheck</span>
                                <div class="tooltip absolute top-20 left-1/2 w-64 p-4 bg-slate-900 text-white text-xs rounded-xl shadow-2xl z-20 pointer-events-none">
                                    <p class="font-bold mb-1 border-b border-white/20 pb-1 uppercase tracking-wider" style="color: #ffdd65;">Eindcheck</p>
                                    <span>Laatste ronde voor inhoud en positionering. Eén centrale ronde!</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Productie Lijn (Groen) -->
                    <div class="relative mb-12 flex items-center h-20">
                        <div class="absolute -left-4 w-32 -translate-x-full text-right pr-4 font-bold text-[10px] uppercase tracking-widest opacity-40">Productie Lijn</div>
                        <div class="absolute left-0 right-0 h-4 rounded-full opacity-20" style="background-color: #61bf89;"></div>
                        <div class="absolute left-0 h-4 rounded-full w-full" style="background-color: #61bf89;"></div>
                        <div class="relative w-full flex justify-between px-10">
                            <div class="station-container relative flex flex-col items-center">
                                <div class="w-12 h-12 rounded-full border-4 border-white shadow-lg flex items-center justify-center z-10 text-slate-900" style="background-color: #61bf89;"><i data-lucide="share-2" size="18"></i></div>
                                <span class="mt-4 font-bold text-[10px] uppercase bg-white px-2 py-1 rounded shadow-sm border border-slate-100">Kanalen</span>
                                <div class="tooltip absolute top-20 left-1/2 w-64 p-4 bg-slate-900 text-white text-xs rounded-xl shadow-2xl z-20 pointer-events-none">
                                    <p class="font-bold mb-1 border-b border-white/20 pb-1 uppercase tracking-wider" style="color: #61bf89;">Kanalen</p>
                                    <span>Kanalen kiezen en beelden op maat maken per platform.</span>
                                </div>
                            </div>
                            <div class="station-container relative flex flex-col items-center">
                                <div class="w-12 h-12 rounded-full border-4 border-white shadow-lg flex items-center justify-center z-10 text-slate-900" style="background-color: #61bf89;"><i data-lucide="mail" size="18"></i></div>
                                <span class="mt-4 font-bold text-[10px] uppercase bg-white px-2 py-1 rounded shadow-sm border border-slate-100">Digitaal</span>
                                <div class="tooltip absolute top-20 left-1/2 w-64 p-4 bg-slate-900 text-white text-xs rounded-xl shadow-2xl z-20 pointer-events-none">
                                    <p class="font-bold mb-1 border-b border-white/20 pb-1 uppercase tracking-wider" style="color: #61bf89;">Digitaal</p>
                                    <span>Verzendlijsten klaarzetten en uploaden naar website/socials.</span>
                                </div>
                            </div>
                            <div class="station-container relative flex flex-col items-center">
                                <div class="w-12 h-12 rounded-full border-4 border-white shadow-lg flex items-center justify-center z-10 text-slate-900" style="background-color: #61bf89;"><i data-lucide="package" size="18"></i></div>
                                <span class="mt-4 font-bold text-[10px] uppercase bg-white px-2 py-1 rounded shadow-sm border border-slate-100">Fysiek</span>
                                <div class="tooltip absolute top-20 left-1/2 w-64 p-4 bg-slate-900 text-white text-xs rounded-xl shadow-2xl z-20 pointer-events-none">
                                    <p class="font-bold mb-1 border-b border-white/20 pb-1 uppercase tracking-wider" style="color: #61bf89;">Fysiek</p>
                                    <span>Drukwerk en verspreiding regelen. Houd rekening met levertijden!</span>
                                </div>
                            </div>
                            <div class="station-container relative flex flex-col items-center">
                                <div class="w-12 h-12 rounded-full border-4 border-white shadow-lg flex items-center justify-center z-10 text-slate-900" style="background-color: #61bf89;"><i data-lucide="train" size="18"></i></div>
                                <span class="mt-4 font-bold text-[10px] uppercase bg-white px-2 py-1 rounded shadow-sm border border-slate-100">LANCERING</span>
                                <div class="tooltip absolute top-20 left-1/2 w-64 p-4 bg-slate-900 text-white text-xs rounded-xl shadow-2xl z-20 pointer-events-none">
                                    <p class="font-bold mb-1 border-b border-white/20 pb-1 uppercase tracking-wider" style="color: #61bf89;">LANCERING</p>
                                    <span>Go Live! Wie drukt op de knop? En wie evalueert de voortgang?</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="absolute left-[85%] top-4 bottom-4 w-6 bg-slate-200 -z-10 opacity-10 rounded-full" style="transform: translateX(-50%);"></div>
                </div>
            </div>

            <!-- Checklist -->
            <div class="bg-slate-50 rounded-2xl p-6 md:p-10 border border-slate-200 shadow-inner">
                <div class="flex items-center gap-3 mb-6 text-slate-900">
                    <i data-lucide="check-circle-2" size="28"></i>
                    <h2 class="text-3xl font-normal font-bebas tracking-wide uppercase border-b-4 pb-1" style="border-color: #5d8c8e;">Check voordat je de trein laat vertrekken</h2>
                </div>
                <p class="text-slate-600 mb-8 italic text-lg">Loop deze vragen door voordat je een communicatie-verzoek indient. Geen volledige antwoorden? Dan blijf je nog even op de blauwe lijn!</p>
                
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-10">
                    <!-- Checklist items -->
                    <div class="flex gap-4 items-start bg-white p-6 rounded-2xl shadow-sm border border-slate-100">
                        <div class="w-8 h-8 rounded-lg mt-1 shrink-0 flex items-center justify-center font-bold border text-white" style="background-color: #5d8c8e; border-color: rgba(0,0,0,0.1);">1</div>
                        <div>
                            <h3 class="font-bold text-slate-800 uppercase text-sm tracking-wide mb-1">Doel & Resultaat</h3>
                            <p class="text-slate-600 text-sm leading-relaxed">Wat is het einddoel? Welke fases zijn er nodig om daar te komen?</p>
                        </div>
                    </div>
                    <div class="flex gap-4 items-start bg-white p-6 rounded-2xl shadow-sm border border-slate-100">
                        <div class="w-8 h-8 rounded-lg mt-1 shrink-0 flex items-center justify-center font-bold border text-white" style="background-color: #5d8c8e; border-color: rgba(0,0,0,0.1);">2</div>
                        <div>
                            <h3 class="font-bold text-slate-800 uppercase text-sm tracking-wide mb-1">Doelgroep</h3>
                            <p class="text-slate-600 text-sm leading-relaxed">Wie zijn ze? Wat weten ze al over burgerberaden en wat nog niet?</p>
                        </div>
                    </div>
                    <div class="flex gap-4 items-start bg-white p-6 rounded-2xl shadow-sm border border-slate-100">
                        <div class="w-8 h-8 rounded-lg mt-1 shrink-0 flex items-center justify-center font-bold border text-white" style="background-color: #5d8c8e; border-color: rgba(0,0,0,0.1);">3</div>
                        <div>
                            <h3 class="font-bold text-slate-800 uppercase text-sm tracking-wide mb-1">Timing</h3>
                            <p class="text-slate-600 text-sm leading-relaxed">6-8 weken voor kleine projecten, 3-12 maanden voor grote trajecten.</p>
                        </div>
                    </div>
                    <div class="flex gap-4 items-start bg-white p-6 rounded-2xl shadow-sm border border-slate-100">
                        <div class="w-8 h-8 rounded-lg mt-1 shrink-0 flex items-center justify-center font-bold border text-white" style="background-color: #5d8c8e; border-color: rgba(0,0,0,0.1);">4</div>
                        <div>
                            <h3 class="font-bold text-slate-800 uppercase text-sm tracking-wide mb-1">Budget & Kaders</h3>
                            <p class="text-slate-600 text-sm leading-relaxed">Is er budget voor een fotograaf, drukwerk of extra copywriter?</p>
                        </div>
                    </div>
                </div>
                
                <!-- Regels -->
                <div class="grid grid-cols-1 lg:grid-cols-3 gap-4">
                    <div class="p-6 bg-white border-l-8 rounded-r-2xl shadow-sm flex flex-col" style="border-color: #5d8c8e;">
                        <h4 class="font-normal font-bebas tracking-wider text-slate-900 uppercase text-xl mb-2">Instap-Instructie:</h4>
                        <p class="text-slate-700 text-base italic leading-tight">"Instappen zonder bestemming (briefing) is avontuurlijk, maar in communicatie-land eindig je dan meestal in een weiland zonder wifi."</p>
                    </div>
                    <div class="p-6 bg-white border-l-8 rounded-r-2xl shadow-sm flex flex-col" style="border-color: #ffdd65;">
                        <h4 class="font-normal font-bebas tracking-wider text-slate-900 uppercase text-xl mb-2">Vormgevers-Vibe:</h4>
                        <p class="text-slate-700 text-base italic leading-tight">"De vormgever is geen tovenaar. Zonder tijdige input wordt het ontwerp 'net niet' – en we willen geen stoptrein-uitstraling!"</p>
                    </div>
                    <div class="p-6 bg-white border-l-8 rounded-r-2xl shadow-sm flex flex-col" style="border-color: #61bf89;">
                        <h4 class="font-normal font-bebas tracking-wider text-slate-900 uppercase text-xl mb-2">Conducteurs Wijsheid:</h4>
                        <p class="text-slate-700 text-base italic leading-tight">"Een 'effe snel' PDF'je om vijf voor vijf? Dat is geen campagne, dat is een noodstop. Zelfs de Thalys moet opstarten."</p>
                    </div>
                </div>
            </div>

            <!-- Footer -->
            <div class="mt-10 flex flex-col md:flex-row justify-between items-center text-slate-500 text-[10px] md:text-xs border-t border-slate-100 pt-8 uppercase font-bold tracking-widest">
                <p>© 2024 Communicatie routekaart van Bureau burgerberaad</p>
                <div class="flex gap-6 mt-4 md:mt-0 uppercase font-tahoma text-slate-400">
                    <span class="flex items-center gap-1"><i data-lucide="clock" size="14"></i> Doorlooptijd: 6 weken - 12 maanden</span>
                    <span class="flex items-center gap-1"><i data-lucide="check-circle-2" size="14"></i> Start pas bij volledige briefing</span>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Initialiseer Lucide iconen
        lucide.createIcons();
    </script>
</body>
</html>
