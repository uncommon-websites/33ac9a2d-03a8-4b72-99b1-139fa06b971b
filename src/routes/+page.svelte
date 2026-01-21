<script lang="ts">
  // Icons
  import { Play, Mic, Music, Wand2, Type, Languages, Video, Share2, ArrowRight, Plus, X, Search, Settings, ChevronRight, ChevronDown, ShieldCheck, Zap, Globe, MessageSquare } from 'lucide-svelte';

  // State for FAQ
  let openFaq = -1;
  const faqs = [
    {
      q: "How does Delphi train my Digital Mind?",
      a: "Delphi ingests your text, audio, and video content to index your knowledge and style. It then trains a model that mirrors your tone and style without 'hallucinating' or improvising without your consent."
    },
    {
      q: "Is my data secure and private?",
      a: "Yes. Your Digital Mind is fully encrypted and securely stored. We never share or sell your data, and your content is never used to train other people's models."
    },
    {
      q: "Where can I deploy my Digital Mind?",
      a: "You can deploy your Mind across the web via a widget, or through SMS, WhatsApp, Slack, and other popular communication channels."
    },
    {
      q: "Can I control what my Digital Mind says?",
      a: "Absolutely. You have full control over the knowledge base and guidelines. Your Digital Mind only uses your own words and guidance to ensure authenticity."
    },
    {
      q: "What is the 'Immortal' offering?",
      a: "Delphi Immortal is designed for top-tier leaders and public figures to preserve their knowledge and persona for future generations, turning their influence into a persistent digital legacy."
    }
  ];

  function toggleFaq(index: number) {
    openFaq = openFaq === index ? -1 : index;
  }
</script>

<main class="w-full overflow-hidden">
  <!-- Hero Section (MATCHING APPROVED REFERENCE) -->
  <section class="w-full px-6 md:px-8 pt-20 pb-16 md:pt-28 md:pb-24">
    <div class="max-w-[1400px] mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12 items-start">
        
        <!-- Headline & CTA -->
        <div class="lg:col-span-7">
            <h1 class="text-4xl md:text-5xl lg:text-6xl leading-[1.1] font-semibold tracking-tight text-gray-900 mb-10">
                Your expertise, scaled. Experience your <br class="hidden lg:block"> Digital Mind.
            </h1>
            <button class="px-8 py-4 bg-black text-white rounded-full text-[17px] font-medium hover:bg-gray-800 transition-transform transform hover:scale-105">
                Get started for free
            </button>
        </div>

        <!-- Subtext -->
        <div class="lg:col-span-5 pt-2 md:pt-4">
            <p style="color: #334155" class="text-lg md:text-[1.25rem] leading-relaxed font-normal">
                Delphi delivers always-on, authentic conversations via encrypted Digital Minds built from your content. Preserve your knowledge and engage your audience 24/7.
            </p>
        </div>
    </div>
  </section>

  <!-- Hero Image / UI Mockup Section (MATCHING APPROVED REFERENCE) -->
  <section class="w-full px-4 pb-10">
    <div class="max-w-[1400px] mx-auto rounded-[32px] bg-gradient-to-br from-[#8ba0f3] via-[#9b9be0] to-[#9c6d8e] p-6 md:p-12 lg:p-20 relative overflow-hidden min-h-[600px] lg:min-h-[800px]">
        
        <!-- UI Container -->
        <div class="bg-white rounded-2xl shadow-2xl overflow-hidden max-w-7xl mx-auto relative z-10">
            
            <!-- UI Header -->
            <div class="flex items-center justify-between px-6 py-4 border-b border-gray-100 bg-white">
                <div class="flex items-center gap-6">
                    <span class="font-semibold text-gray-800 text-sm">Digital Mind 1.0</span>
                    <div class="flex items-center gap-4 text-gray-400">
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 14 4 9l5-5"/><path d="M4 9h10.5a5.5 5.5 0 0 1 5.5 5.5v0a5.5 5.5 0 0 1-5.5 5.5H11"/></svg>
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m15 14 5-5-5-5"/><path d="M20 9H9.5A5.5 5.5 0 0 0 4 14.5v0A5.5 5.5 0 0 0 9.5 20H13"/></svg>
                    </div>
                </div>
                <div class="flex items-center gap-4">
                    <span class="text-gray-500 text-sm font-medium cursor-pointer hover:text-gray-800">Share</span>
                    <button style="background-color: #4f46e5" class="text-white px-4 py-1.5 rounded-lg text-xs font-bold tracking-wide">Export</button>
                </div>
            </div>

            <!-- UI Body -->
            <div class="flex flex-col lg:flex-row h-[600px] bg-white">
                
                <!-- Left: Text Editor -->
                <div class="w-full lg:w-1/2 p-8 lg:p-12 overflow-y-auto border-r border-gray-100 no-scrollbar">
                    <div class="flex gap-4 mb-8">
                        <div class="mt-1.5 w-3 h-3 rounded-full bg-gradient-to-br from-blue-400 to-blue-600 flex-shrink-0"></div>
                        <div class="border-l-2 border-gray-800 pl-4">
                            <p class="font-semibold text-gray-900 text-lg">Delphi AI proudly introduces Digital Minds.</p>
                        </div>
                    </div>

                    <div class="flex gap-4 mb-8">
                        <div class="w-3 flex-shrink-0"></div>
                        <div class="border-l-2 border-gray-200 pl-4">
                            <p class="text-gray-500 text-base leading-relaxed">
                                Your Digital Mind is a persistent, interactive representation of your knowledge and persona. Built from your audio, video, and text.
                            </p>
                        </div>
                    </div>

                    <div class="flex gap-4 mb-8">
                        <div class="w-3 flex-shrink-0"></div>
                        <div class="border-l-2 border-gray-300 pl-4">
                            <p class="text-gray-400 text-base leading-relaxed">
                                Deploy your Mind to Slack, WhatsApp, and the web. Your audience can talk to you anytime, anywhere, while preserving your style.
                            </p>
                        </div>
                    </div>

                    <div class="flex gap-4">
                        <div class="w-3 flex-shrink-0"></div>
                        <div class="border-l-2 border-gray-200 pl-4">
                            <p class="text-gray-300 text-base leading-relaxed">
                                Securely encrypted and fully private.
                            </p>
                        </div>
                    </div>
                </div>

                <!-- Right: Visual Preview -->
                <div class="w-full lg:w-1/2 bg-gray-50 p-8 lg:p-12 flex items-center justify-center relative">
                    <div class="w-full h-full relative rounded-lg overflow-hidden shadow-lg bg-gray-200">
                        <img src="/generated/image-a-high-end-minimalist-workspace-with-a-s-1769023849819-0.webp" alt="Studio Preview" class="w-full h-full object-cover">
                        <div class="absolute inset-0 bg-gradient-to-tr from-blue-600/40 via-transparent to-orange-500/40 opacity-80 mix-blend-multiply"></div>
                    </div>
                    <div class="absolute right-4 top-1/2 -translate-y-1/2 flex flex-col gap-6 text-gray-400">
                        <button class="p-2 hover:bg-white hover:shadow-sm rounded-lg transition-all"><Zap size={20} /></button>
                        <button class="p-2 hover:bg-white hover:shadow-sm rounded-lg transition-all"><ShieldCheck size={20} /></button>
                        <button class="p-2 hover:bg-white hover:shadow-sm rounded-lg transition-all"><Settings size={20} /></button>
                    </div>
                </div>
            </div>
        </div>

        <!-- Floating Voice Chat Widget -->
        <div class="absolute bottom-8 right-8 md:bottom-12 md:right-12 z-20">
            <div class="bg-white rounded-full p-1.5 shadow-[0_8px_30px_rgb(0,0,0,0.12)] flex items-center gap-2 pr-4">
                <div class="w-10 h-10 rounded-full bg-gradient-to-br from-cyan-400 to-blue-600 flex items-center justify-center relative overflow-hidden">
                    <div class="absolute inset-0 bg-white opacity-20 rotate-45 transform translate-x-1/2"></div>
                </div>
                <button style="background-color: #4f46e5" class="text-white text-[11px] font-bold px-4 py-2 rounded-full flex items-center gap-2 tracking-wider">
                    <Mic size={12} />
                    TALK TO MIND
                </button>
                <div class="flex items-center gap-1 ml-1 cursor-pointer">
                    <div class="w-5 h-5 rounded-full overflow-hidden border border-gray-200">
                        <img src="https://flagcdn.com/w20/us.png" alt="US Flag" class="w-full h-full object-cover">
                    </div>
                    <ChevronDown size={12} class="text-gray-500" />
                </div>
            </div>
            <div class="text-[10px] text-gray-500 text-right mt-2 pr-2 opacity-60">
                Powered by Delphi AI Digital Minds
            </div>
        </div>
    </div>
  </section>

  <!-- Intro Section -->
  <section class="max-w-[1000px] mx-auto px-6 py-24 text-center">
    <span class="text-sm font-medium text-primary-600 mb-4 block">Introducing Digital Minds 2.0</span>
    <h2 class="text-4xl md:text-5xl font-medium tracking-tight mb-8 leading-tight">
      Be everywhere, without doing everything. Delphi turns your expertise into an always-on interactive experience.
    </h2>
    
    <div class="flex flex-wrap justify-center gap-x-6 gap-y-3 text-sm text-gray-600 mb-10">
      <span class="flex items-center gap-2 px-3 py-1 bg-gray-50 rounded-full border border-gray-100"><ShieldCheck size={14} /> Fully Encrypted</span>
      <span class="flex items-center gap-2 px-3 py-1 bg-gray-50 rounded-full border border-gray-100"><Zap size={14} /> Zero Latency</span>
      <span class="flex items-center gap-2 px-3 py-1 bg-gray-50 rounded-full border border-gray-100"><Globe size={14} /> Multi-channel</span>
      <span class="flex items-center gap-2 px-3 py-1 bg-gray-50 rounded-full border border-gray-100"><MessageSquare size={14} /> Authentic Voice</span>
      <span class="flex items-center gap-2 px-3 py-1 bg-gray-50 rounded-full border border-gray-100"><Share2 size={14} /> Viral Distribution</span>
    </div>

    <button class="inline-flex items-center gap-2 bg-black text-white pl-3 pr-5 py-2 rounded-full text-sm font-medium hover:bg-gray-800 transition-colors">
      <div class="w-6 h-6 bg-white rounded-full flex items-center justify-center">
        <Play size={10} class="fill-black text-black ml-0.5" />
      </div>
      See how it works
    </button>
  </section>

  <!-- Features List Section -->
  <section class="max-w-[1400px] mx-auto px-6 py-12 relative">
    <div class="grid grid-cols-1 md:grid-cols-2 gap-24">
        
        <!-- Feature 1 -->
        <div class="flex flex-col justify-center order-1 md:order-1">
            <h3 class="text-3xl font-medium mb-4">Your knowledge, indexed</h3>
            <p class="text-gray-600 leading-relaxed mb-6">
                Delphi ingests your podcasts, blogs, videos, and books to build a comprehensive knowledge base. Your Digital Mind speaks only with your words, ensuring every interaction is 100% authentic to your expertise.
            </p>
        </div>
        <div class="bg-gray-50 rounded-2xl p-6 border border-gray-100 order-2 md:order-2">
            <div class="text-xs text-gray-400 mb-4 font-medium uppercase tracking-wide">Connected Sources</div>
            <div class="space-y-3">
                {#each [
                    {name: "The Knowledge Project", desc: "Podcast • 124 Episodes", icon: Mic},
                    {name: "Principles for Success", desc: "Book • Full Text", icon: Type},
                    {name: "Weekly Newsletter", desc: "Blog • 250+ Articles", icon: Share2},
                    {name: "YouTube Channel", desc: "Video • 45 Videos", icon: Video},
                ] as source}
                <div class="flex items-center gap-3 p-3 bg-white rounded-lg border border-gray-100 shadow-sm">
                    <div class="w-10 h-10 rounded-full bg-primary-50 flex items-center justify-center text-primary-600">
                        <source.icon size={20} />
                    </div>
                    <div>
                        <div class="text-sm font-medium text-gray-900">{source.name}</div>
                        <div class="text-xs text-gray-500">{source.desc}</div>
                    </div>
                    <div class="ml-auto">
                        <div class="px-2 py-1 bg-green-50 text-green-600 text-[10px] font-bold rounded uppercase">Synced</div>
                    </div>
                </div>
                {/each}
            </div>
        </div>

        <!-- Feature 2 -->
        <div class="bg-gray-50 rounded-2xl p-6 border border-gray-100 min-h-[400px] flex items-center justify-center order-4 md:order-3 relative overflow-hidden">
             <img src="/generated/image-a-diverse-group-of-professional-creators-1769023852455-1.webp" alt="Creators" class="absolute inset-0 w-full h-full object-cover opacity-20" />
             <div class="relative z-10 text-center p-8">
                 <div class="w-20 h-20 bg-white rounded-full flex items-center justify-center mx-auto mb-6 shadow-xl">
                     <Globe size={32} class="text-primary-600" />
                 </div>
                 <h4 class="text-xl font-medium mb-2">Deploy Anywhere</h4>
                 <p class="text-sm text-gray-600">Web, WhatsApp, Slack, SMS, and more.</p>
             </div>
        </div>
        <div class="flex flex-col justify-center order-3 md:order-4">
            <h3 class="text-3xl font-medium mb-4">Meet your audience where they are</h3>
            <p class="text-gray-600 leading-relaxed">
                Scale your presence across every major communication channel. Whether it's a private WhatsApp for high-ticket coaching or a public web widget for your fans, your Digital Mind is always ready to engage.
            </p>
        </div>

        <!-- Feature 3 -->
        <div class="flex flex-col justify-center order-5 md:order-5">
            <h3 class="text-3xl font-medium mb-4">Privacy first, by design</h3>
            <p class="text-gray-600 leading-relaxed">
                Your data is your legacy. We use enterprise-grade encryption and strict privacy controls. Your content is never used to train other models, and your Digital Mind is yours alone.
            </p>
        </div>
        <div class="bg-gray-50 rounded-2xl p-6 border border-gray-100 min-h-[300px] flex items-center justify-center order-6 md:order-6">
             <div class="w-full max-w-xs bg-white rounded-xl shadow-sm p-6 border border-gray-100 text-center">
                 <div class="w-12 h-12 bg-primary-100 rounded-lg flex items-center justify-center text-primary-600 mx-auto mb-4">
                     <ShieldCheck size={24} />
                 </div>
                 <div class="text-sm font-medium mb-1">End-to-End Encryption</div>
                 <div class="text-xs text-gray-500 mb-4">Your knowledge is secured with AES-256</div>
                 <div class="h-1.5 bg-gray-100 rounded-full overflow-hidden">
                     <div class="h-full bg-primary-500 w-full"></div>
                 </div>
             </div>
        </div>
    </div>
  </section>
  
  <!-- Floating Action Bar -->
  <div class="sticky bottom-6 z-40 flex justify-center pointer-events-none">
      <div class="bg-white/80 backdrop-blur-md border border-gray-200 shadow-lg rounded-full py-3 px-6 flex items-center gap-6 pointer-events-auto">
          <span class="text-sm font-medium text-gray-900 hidden sm:block">Ready to scale your expertise?</span>
          <button class="bg-black text-white text-xs font-bold px-4 py-2 rounded-full hover:bg-gray-800 transition-colors">
              Get Started
          </button>
      </div>
  </div>

  <!-- Built for Every Expert -->
  <section class="max-w-[1400px] mx-auto px-6 py-24">
      <div class="text-center max-w-2xl mx-auto mb-16">
        <h2 class="text-4xl font-medium tracking-tight mb-4">Trusted by leading minds</h2>
        <p class="text-gray-600">Delphi helps high-trust voices meet high-demand audiences without scaling complexity.</p>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <!-- Creator 1 -->
        <div class="group">
            <div class="aspect-square rounded-2xl overflow-hidden mb-6 relative">
                <img src="/generated/image-a-close-up-portrait-of-a-confident-frien-1769023854472-2.webp" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" alt="Expert" />
                <div class="absolute inset-0 bg-gradient-to-t from-primary-900/60 to-transparent mix-blend-multiply"></div>
                <div class="absolute inset-0 bg-primary-500/20 mix-blend-color"></div>
            </div>
            <h3 class="text-lg font-medium mb-2">Bestselling Authors</h3>
            <p class="text-xs text-gray-500 leading-relaxed">Let readers engage with your work directly. Your Digital Mind can answer questions about your books 24/7, providing a personalized reading companion.</p>
        </div>

        <!-- Creator 2 -->
        <div class="group">
            <div class="aspect-square rounded-2xl overflow-hidden mb-6 relative">
                <img src="/generated/image-a-close-up-portrait-of-a-thoughtful-crea-1769023856453-3.webp" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" alt="Coach" />
                <div class="absolute inset-0 bg-gradient-to-t from-gray-900/60 to-transparent mix-blend-multiply"></div>
                <div class="absolute inset-0 bg-gray-500/20 mix-blend-color"></div>
            </div>
            <h3 class="text-lg font-medium mb-2">Executive Coaches</h3>
            <p class="text-xs text-gray-500 leading-relaxed">Offer private guidance around the clock. Your Digital Mind provides instant support to your clients between sessions, scaling your impact.</p>
        </div>

        <!-- Creator 3 -->
        <div class="group">
            <div class="aspect-square rounded-2xl overflow-hidden mb-6 relative">
                <img src="https://images.unsplash.com/photo-1590602847861-f357a9332bbc?q=80&w=2070&auto=format&fit=crop" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" alt="Podcaster" />
                <div class="absolute inset-0 bg-gradient-to-t from-primary-900/60 to-transparent mix-blend-multiply"></div>
                <div class="absolute inset-0 bg-primary-500/20 mix-blend-color"></div>
            </div>
            <h3 class="text-lg font-medium mb-2">Podcasters & Creators</h3>
            <p class="text-xs text-gray-500 leading-relaxed">Answer follow-up questions automatically. Turn your episodes into an interactive knowledge base that fans can talk to anytime.</p>
        </div>
    </div>
  </section>

  <!-- FAQ Section -->
  <section class="max-w-[1000px] mx-auto px-6 py-24">
      <h2 class="text-3xl font-medium mb-12">Frequently asked questions</h2>
      
      <div class="divide-y divide-gray-100">
          {#each faqs as faq, i}
            <div class="py-4">
                <button class="w-full flex items-center justify-between text-left group" on:click={() => toggleFaq(i)}>
                    <span class="text-sm md:text-base text-gray-700 group-hover:text-black transition-colors">{faq.q}</span>
                    <span class="text-gray-400">
                        <Plus size={16} class="transition-transform duration-200 {openFaq === i ? 'rotate-45' : ''}" />
                    </span>
                </button>
                {#if openFaq === i}
                    <div class="mt-4 text-sm text-gray-500 leading-relaxed pb-2">
                        {faq.a}
                    </div>
                {#/if}
            </div>
          {/each}
      </div>
  </section>

  <!-- Bottom CTA -->
  <section class="max-w-[1400px] mx-auto px-6 py-24 flex flex-col items-center text-center border-t border-gray-100">
      <h2 class="text-4xl font-medium tracking-tight mb-8">The most authentic Digital Mind platform</h2>
      <div class="flex items-center gap-4">
          <button class="bg-black text-white px-6 py-3 rounded-full font-medium hover:bg-gray-800 transition-colors text-sm">
              Create your Digital Mind
          </button>
          <button class="bg-white text-black border border-gray-200 px-6 py-3 rounded-full font-medium hover:bg-gray-50 transition-colors text-sm">
              Talk to sales
          </button>
      </div>
  </section>
</main>

<style>
    .no-scrollbar::-webkit-scrollbar {
        display: none;
    }
    .no-scrollbar {
        -ms-overflow-style: none;
        scrollbar-width: none;
    }
</style>