export default function LielPortfolioLanding() {
  const projects = [
    {
      title: "Grandma’s Recipes, Frontend",
      stack: "Vue.js · REST API · Bootstrap · Axios",
      description:
        "Multi-page recipe platform with modular UI architecture, client-side routing, personalized recipe flows, favorites, and meal-planning interactions.",
      link: "#",
      category: "Frontend",
    },
    {
      title: "Grandma’s Recipes, Backend",
      stack: "Node.js · Express · MySQL · REST API",
      description:
        "Backend service handling authentication, session flows, persistence, and integration with external recipe data sources.",
      link: "#",
      category: "Backend",
    },
    {
      title: "Network Speed Test Service",
      stack: "Python · TCP/UDP · Sockets · Threading",
      description:
        "Networking project focused on concurrent transfer testing, custom protocol messages, and performance measurement across TCP and UDP.",
      link: "#",
      category: "Systems",
    },
    {
      title: "Aunt Lucy Landing Page",
      stack: "HTML · CSS · JavaScript",
      description:
        "Character-driven landing page with soft visual language, storytelling, gallery, playlist, interactive poll, and polished client-side details.",
      link: "#",
      category: "Design",
    },
  ];

  const skills = {
    frontend: ["Vue.js", "React", "JavaScript", "HTML", "CSS", "Responsive UI", "Component Design"],
    backend: ["Node.js", "Express", "REST APIs", "MySQL", "Session Management", "API Integration"],
    general: ["Git", "Debugging", "Teamwork", "Modular Development", "Project Delivery"],
  };

  return (
    <div className="min-h-screen bg-[#fbf7f2] text-[#4d4038]">
      <div className="absolute inset-0 -z-10 overflow-hidden">
        <div className="absolute left-0 top-0 h-80 w-80 rounded-full bg-[#f4dfd2] blur-3xl opacity-70" />
        <div className="absolute right-0 top-32 h-96 w-96 rounded-full bg-[#efe5d6] blur-3xl opacity-80" />
        <div className="absolute bottom-0 left-1/3 h-80 w-80 rounded-full bg-[#e7d7c5] blur-3xl opacity-60" />
      </div>

      <header className="sticky top-0 z-20 border-b border-[#eadfd3] bg-[#fbf7f2]/85 backdrop-blur">
        <div className="mx-auto flex max-w-6xl items-center justify-between px-6 py-4">
          <div>
            <p className="text-sm tracking-[0.18em] uppercase text-[#a38c7c]">Portfolio</p>
            <h1 className="text-2xl font-semibold tracking-tight text-[#4d4038]">Liel Parparov</h1>
          </div>
          <nav className="hidden items-center gap-6 text-sm text-[#7f6e62] md:flex">
            <a href="#about" className="transition hover:text-[#4d4038]">About</a>
            <a href="#projects" className="transition hover:text-[#4d4038]">Projects</a>
            <a href="#skills" className="transition hover:text-[#4d4038]">Skills</a>
            <a href="#contact" className="transition hover:text-[#4d4038]">Contact</a>
          </nav>
        </div>
      </header>

      <main>
        <section className="mx-auto grid max-w-6xl gap-12 px-6 py-20 md:grid-cols-[1.15fr_0.85fr] md:py-28 items-center">
          <div>
            <p className="inline-flex items-center rounded-full border border-[#e7d7cb] bg-white/80 px-4 py-2 text-sm text-[#8b7769] shadow-sm">
              Junior Full Stack Developer
            </p>
            <h2 className="mt-6 max-w-3xl text-4xl font-semibold leading-tight tracking-tight text-[#4c3d35] md:text-6xl">
              Building thoughtful products with a strong frontend eye and clean full stack execution.
            </h2>
            <p className="mt-6 max-w-2xl text-lg leading-8 text-[#6f6055]">
              Software & Information Systems Engineering graduate from Ben-Gurion University, with hands-on experience in frontend development, API integration, and full stack academic projects. I care about polished interfaces, clear structure, and reliable implementation.
            </p>
            <div className="mt-8 flex flex-wrap gap-4">
              <a
                href="#projects"
                className="rounded-full bg-[#c98f78] px-6 py-3 text-white shadow-sm transition hover:bg-[#b97f69]"
              >
                View Projects
              </a>
              <a
                href="#contact"
                className="rounded-full border border-[#dccbbd] bg-white px-6 py-3 text-[#5f4f45] transition hover:bg-[#f7efe8]"
              >
                Contact
              </a>
            </div>
          </div>

          <div className="grid gap-5">
            <div className="rounded-[2rem] border border-[#eadfd3] bg-white/90 p-7 shadow-[0_18px_50px_rgba(113,91,74,0.08)]">
              <p className="text-sm uppercase tracking-[0.18em] text-[#a38c7c]">Focus Areas</p>
              <div className="mt-5 flex flex-wrap gap-3">
                {['Vue.js', 'Frontend Architecture', 'REST APIs', 'Node.js', 'MySQL', 'UI Systems'].map((item) => (
                  <span
                    key={item}
                    className="rounded-full bg-[#f8efe7] px-4 py-2 text-sm text-[#6e5f54]"
                  >
                    {item}
                  </span>
                ))}
              </div>
            </div>
            <div className="rounded-[2rem] border border-[#eadfd3] bg-[#f6ede5] p-7 shadow-[0_18px_50px_rgba(113,91,74,0.08)]">
              <p className="text-sm uppercase tracking-[0.18em] text-[#a38c7c]">Highlights</p>
              <ul className="mt-5 space-y-3 text-[#6b5a4f] leading-7">
                <li>Led frontend implementation in multi-page academic projects</li>
                <li>Built modular interfaces and connected them to backend APIs</li>
                <li>Worked across web, backend, networking, and UI-driven coursework</li>
              </ul>
            </div>
          </div>
        </section>

        <section id="about" className="mx-auto max-w-6xl px-6 py-6">
          <div className="rounded-[2.25rem] border border-[#eadfd3] bg-white/90 p-8 shadow-[0_18px_50px_rgba(113,91,74,0.06)] md:p-10">
            <p className="text-sm uppercase tracking-[0.18em] text-[#a38c7c]">About</p>
            <div className="mt-5 grid gap-8 md:grid-cols-[1.25fr_0.75fr]">
              <p className="text-lg leading-8 text-[#6c5d53]">
                I enjoy creating interfaces that feel refined, structured, and intentional. My work combines strong frontend ownership with practical backend integration, and I am especially drawn to projects where design quality, usability, and implementation discipline all matter.
              </p>
              <div className="rounded-[1.75rem] border border-[#eee1d6] bg-[#faf3ec] p-6">
                <p className="text-base font-semibold text-[#4d4038]">Currently looking for</p>
                <p className="mt-3 leading-7 text-[#6f6055]">
                  A junior full stack or frontend-oriented role where I can contribute, grow, and keep building reliable user-facing systems.
                </p>
              </div>
            </div>
          </div>
        </section>

        <section id="projects" className="mx-auto max-w-6xl px-6 py-20">
          <div>
            <p className="text-sm uppercase tracking-[0.18em] text-[#a38c7c]">Selected Work</p>
            <h3 className="mt-3 text-3xl font-semibold tracking-tight text-[#4c3d35] md:text-4xl">Projects</h3>
          </div>

          <div className="mt-10 grid gap-6 md:grid-cols-2">
            {projects.map((project) => (
              <article
                key={project.title}
                className="rounded-[2rem] border border-[#eadfd3] bg-white/90 p-8 shadow-[0_18px_50px_rgba(113,91,74,0.06)] transition hover:-translate-y-1 hover:shadow-[0_22px_60px_rgba(113,91,74,0.10)]"
              >
                <div className="flex items-start justify-between gap-4">
                  <div>
                    <span className="rounded-full bg-[#f8efe7] px-3 py-1 text-xs uppercase tracking-[0.18em] text-[#a07f6d]">
                      {project.category}
                    </span>
                    <h4 className="mt-4 text-2xl font-semibold tracking-tight text-[#4d4038]">{project.title}</h4>
                    <p className="mt-2 text-sm text-[#9a8679]">{project.stack}</p>
                  </div>
                </div>
                <p className="mt-5 text-lg leading-8 text-[#6e5f54]">{project.description}</p>
                <a
                  href={project.link}
                  className="mt-6 inline-flex rounded-full border border-[#dccbbd] px-4 py-2 text-sm text-[#5f4f45] transition hover:bg-[#f7efe8]"
                >
                  View Repository
                </a>
              </article>
            ))}
          </div>
        </section>

        <section id="skills" className="mx-auto max-w-6xl px-6 pb-20">
          <div className="rounded-[2.25rem] border border-[#eadfd3] bg-white/90 p-8 shadow-[0_18px_50px_rgba(113,91,74,0.06)] md:p-10">
            <p className="text-sm uppercase tracking-[0.18em] text-[#a38c7c]">Skills</p>
            <div className="mt-8 grid gap-6 md:grid-cols-3">
              <div className="rounded-[1.5rem] bg-[#fcf6f0] p-6">
                <h4 className="text-lg font-semibold text-[#4d4038]">Frontend</h4>
                <div className="mt-4 flex flex-wrap gap-2">
                  {skills.frontend.map((skill) => (
                    <span key={skill} className="rounded-full bg-white px-3 py-2 text-sm text-[#6a5a50] shadow-sm">
                      {skill}
                    </span>
                  ))}
                </div>
              </div>
              <div className="rounded-[1.5rem] bg-[#f9f1ea] p-6">
                <h4 className="text-lg font-semibold text-[#4d4038]">Backend</h4>
                <div className="mt-4 flex flex-wrap gap-2">
                  {skills.backend.map((skill) => (
                    <span key={skill} className="rounded-full bg-white px-3 py-2 text-sm text-[#6a5a50] shadow-sm">
                      {skill}
                    </span>
                  ))}
                </div>
              </div>
              <div className="rounded-[1.5rem] bg-[#f6ede5] p-6">
                <h4 className="text-lg font-semibold text-[#4d4038]">General</h4>
                <div className="mt-4 flex flex-wrap gap-2">
                  {skills.general.map((skill) => (
                    <span key={skill} className="rounded-full bg-white px-3 py-2 text-sm text-[#6a5a50] shadow-sm">
                      {skill}
                    </span>
                  ))}
                </div>
              </div>
            </div>
          </div>
        </section>

        <section id="contact" className="mx-auto max-w-6xl px-6 pb-24">
          <div className="rounded-[2.25rem] border border-[#decfc3] bg-gradient-to-br from-[#d8b6a4] via-[#cfa895] to-[#bb8f7d] p-8 text-white shadow-[0_24px_70px_rgba(140,100,82,0.20)] md:p-10">
            <p className="text-sm uppercase tracking-[0.18em] text-white/70">Contact</p>
            <h3 className="mt-3 text-3xl font-semibold tracking-tight md:text-4xl">Let’s connect</h3>
            <p className="mt-4 max-w-2xl text-lg leading-8 text-white/85">
              Open to junior software roles, frontend-focused opportunities, and full stack positions where product quality and clean implementation matter.
            </p>
            <div className="mt-8 flex flex-wrap gap-4">
              <a
                href="mailto:your.email@example.com"
                className="rounded-full bg-white px-6 py-3 text-[#8e6757] transition hover:opacity-90"
              >
                Email Me
              </a>
              <a
                href="https://github.com/"
                className="rounded-full border border-white/40 px-6 py-3 text-white transition hover:bg-white/10"
              >
                GitHub
              </a>
              <a
                href="https://www.linkedin.com/"
                className="rounded-full border border-white/40 px-6 py-3 text-white transition hover:bg-white/10"
              >
                LinkedIn
              </a>
            </div>
          </div>
        </section>
      </main>
    </div>
  );
}
