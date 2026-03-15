export default function LielPortfolioLanding() {
  const projects = [
    {
      title: "Grandma's Recipes, Frontend",
      stack: "Vue.js · REST API · Bootstrap · Axios",
      description:
        "Multi-page recipe management client with modular UI architecture, dynamic routing, favorites, meal planning, and personalized recipe flows.",
      link: "#",
      emoji: "🍽️",
    },
    {
      title: "Grandma's Recipes, Backend",
      stack: "Node.js · Express · MySQL · REST API",
      description:
        "Server-side application handling authentication, session management, database persistence, and integration with external recipe data.",
      link: "#",
      emoji: "🛠️",
    },
    {
      title: "Network Speed Test Service",
      stack: "Python · TCP/UDP · Sockets · Threading",
      description:
        "Network service for server discovery, concurrent transfer testing, and protocol-level performance measurement using custom binary messages.",
      link: "#",
      emoji: "🚀",
    },
    {
      title: "Aunt Lucy Landing Page",
      stack: "HTML · CSS · JavaScript",
      description:
        "Character-driven landing page with storytelling, gallery, playlist, poll interactions, and a warm visual identity.",
      link: "#",
      emoji: "🧸",
    },
  ];

  return (
    <div className="min-h-screen bg-slate-50 text-slate-900">
      <header className="border-b border-slate-200 bg-white/90 backdrop-blur sticky top-0 z-20">
        <div className="mx-auto max-w-6xl px-6 py-4 flex items-center justify-between">
          <div>
            <p className="text-sm text-slate-500">Software & Information Systems Engineering</p>
            <h1 className="text-2xl font-semibold tracking-tight">Liel Parparov</h1>
          </div>
          <nav className="hidden md:flex items-center gap-6 text-sm text-slate-600">
            <a href="#about" className="hover:text-slate-900">About</a>
            <a href="#projects" className="hover:text-slate-900">Projects</a>
            <a href="#skills" className="hover:text-slate-900">Skills</a>
            <a href="#contact" className="hover:text-slate-900">Contact</a>
          </nav>
        </div>
      </header>

      <main>
        <section className="mx-auto max-w-6xl px-6 py-20 md:py-28 grid md:grid-cols-2 gap-12 items-center">
          <div>
            <p className="inline-flex items-center rounded-full border border-slate-200 bg-white px-4 py-1.5 text-sm text-slate-600 shadow-sm">
              Junior Full Stack Developer
            </p>
            <h2 className="mt-6 text-4xl md:text-6xl font-semibold leading-tight tracking-tight">
              Building clean, thoughtful web products with strong frontend ownership.
            </h2>
            <p className="mt-6 text-lg leading-8 text-slate-600 max-w-xl">
              Software & Information Systems Engineering graduate from Ben-Gurion University, with hands-on experience in frontend development, API integration, and full-stack academic projects.
            </p>
            <div className="mt-8 flex flex-wrap gap-4">
              <a href="#projects" className="rounded-2xl bg-slate-900 px-6 py-3 text-white shadow-sm hover:opacity-90">
                View Projects
              </a>
              <a href="#contact" className="rounded-2xl border border-slate-300 bg-white px-6 py-3 text-slate-700 hover:bg-slate-100">
                Contact
              </a>
            </div>
          </div>

          <div className="grid gap-4">
            <div className="rounded-3xl border border-slate-200 bg-white p-6 shadow-sm">
              <p className="text-sm text-slate-500">Focus Areas</p>
              <div className="mt-4 flex flex-wrap gap-3">
                {['Vue.js', 'React', 'Node.js', 'REST APIs', 'MySQL', 'UI Architecture'].map((item) => (
                  <span key={item} className="rounded-full bg-slate-100 px-4 py-2 text-sm text-slate-700">
                    {item}
                  </span>
                ))}
              </div>
            </div>
            <div className="rounded-3xl border border-slate-200 bg-gradient-to-br from-white to-slate-100 p-6 shadow-sm">
              <p className="text-sm text-slate-500">Highlights</p>
              <ul className="mt-4 space-y-3 text-slate-700">
                <li>Led frontend work in multi-page course projects</li>
                <li>Built modular UI flows and integrated backend APIs</li>
                <li>Worked across web, networking, and interactive design projects</li>
              </ul>
            </div>
          </div>
        </section>

        <section id="about" className="mx-auto max-w-6xl px-6 py-8">
          <div className="rounded-[2rem] border border-slate-200 bg-white p-8 md:p-10 shadow-sm">
            <p className="text-sm uppercase tracking-[0.2em] text-slate-400">About</p>
            <div className="mt-4 grid md:grid-cols-[1.2fr_0.8fr] gap-8">
              <p className="text-lg leading-8 text-slate-600">
                I enjoy building interfaces that feel polished, structured, and easy to use. My background combines strong frontend practice with hands-on backend integration, and I am especially drawn to projects where product thinking and implementation quality matter equally.
              </p>
              <div className="rounded-3xl bg-slate-50 p-6 border border-slate-200">
                <p className="font-medium">Currently looking for</p>
                <p className="mt-2 text-slate-600">A junior full stack or frontend-oriented role where I can contribute, grow, and keep building reliable user-facing systems.</p>
              </div>
            </div>
          </div>
        </section>

        <section id="projects" className="mx-auto max-w-6xl px-6 py-20">
          <div className="flex items-end justify-between gap-6 flex-wrap">
            <div>
              <p className="text-sm uppercase tracking-[0.2em] text-slate-400">Selected Work</p>
              <h3 className="mt-3 text-3xl md:text-4xl font-semibold tracking-tight">Projects</h3>
            </div>
          </div>

          <div className="mt-10 grid gap-6">
            {projects.map((project) => (
              <article key={project.title} className="rounded-[2rem] border border-slate-200 bg-white p-8 shadow-sm hover:shadow-md transition-shadow">
                <div className="flex items-start justify-between gap-4 flex-wrap">
                  <div>
                    <h4 className="text-2xl font-semibold tracking-tight flex items-center gap-3">
                      <span>{project.emoji}</span>
                      <span>{project.title}</span>
                    </h4>
                    <p className="mt-2 text-sm text-slate-500">{project.stack}</p>
                  </div>
                  <a href={project.link} className="rounded-full border border-slate-300 px-4 py-2 text-sm text-slate-700 hover:bg-slate-100">
                    View Repository
                  </a>
                </div>
                <p className="mt-5 max-w-3xl text-lg leading-8 text-slate-600">{project.description}</p>
              </article>
            ))}
          </div>
        </section>

        <section id="skills" className="mx-auto max-w-6xl px-6 pb-20">
          <div className="rounded-[2rem] border border-slate-200 bg-white p-8 md:p-10 shadow-sm">
            <p className="text-sm uppercase tracking-[0.2em] text-slate-400">Skills</p>
            <div className="mt-6 grid md:grid-cols-3 gap-6">
              <div>
                <h4 className="font-semibold text-lg">Frontend</h4>
                <p className="mt-3 text-slate-600 leading-7">Vue.js, React, HTML, CSS, JavaScript, responsive UI, component design, client-side routing.</p>
              </div>
              <div>
                <h4 className="font-semibold text-lg">Backend</h4>
                <p className="mt-3 text-slate-600 leading-7">Node.js, Express, REST APIs, MySQL, session-based flows, API integration.</p>
              </div>
              <div>
                <h4 className="font-semibold text-lg">General</h4>
                <p className="mt-3 text-slate-600 leading-7">Git, teamwork, debugging, modular development, academic project delivery under deadlines.</p>
              </div>
            </div>
          </div>
        </section>

        <section id="contact" className="mx-auto max-w-6xl px-6 pb-24">
          <div className="rounded-[2rem] border border-slate-200 bg-slate-900 text-white p-8 md:p-10 shadow-sm">
            <p className="text-sm uppercase tracking-[0.2em] text-slate-400">Contact</p>
            <h3 className="mt-3 text-3xl md:text-4xl font-semibold tracking-tight">Let’s connect</h3>
            <p className="mt-4 max-w-2xl text-slate-300 text-lg leading-8">
              Open to junior software roles, frontend-focused opportunities, and full-stack positions where product quality and clean implementation matter.
            </p>
            <div className="mt-8 flex flex-wrap gap-4">
              <a href="mailto:your.email@example.com" className="rounded-2xl bg-white px-6 py-3 text-slate-900 hover:opacity-90">
                Email Me
              </a>
              <a href="https://github.com/" className="rounded-2xl border border-slate-700 px-6 py-3 text-white hover:bg-slate-800">
                GitHub
              </a>
              <a href="https://www.linkedin.com/" className="rounded-2xl border border-slate-700 px-6 py-3 text-white hover:bg-slate-800">
                LinkedIn
              </a>
            </div>
          </div>
        </section>
      </main>
    </div>
  );
}
