import React from 'react';

const Profile = () => {
  return (
    <div className="max-w-5xl mx-auto px-4 py-10 text-white bg-gray-900 min-h-screen">
      <h1 className="text-4xl font-bold text-center mb-4">Hi 👋, I'm Sevindi Maleesha Jayathilake</h1>
      <h2 className="text-xl font-semibold text-center text-gray-400 mb-6">
        🚀 IT Undergraduate | SLIIT | Full-Stack Developer in Progress
      </h2>

      <div className="flex justify-center mb-10">
        <img
          src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=22&pause=1000&center=true&vCenter=true&width=435&lines=Passionate+about+Tech+%F0%9F%92%BB;Full-Stack+Learner+%F0%9F%92%BC;Always+learning+something+new+%F0%9F%93%9A"
          alt="Typing SVG"
        />
      </div>

      <div className="flex flex-col md:flex-row items-center gap-6 mb-10">
        <div className="md:w-1/2 space-y-4">
          <h3 className="text-2xl font-semibold">🧠 Currently Learning:</h3>
          <ul className="list-disc list-inside text-gray-300 space-y-1">
            <li>Languages: Java | Python | Kotlin | JavaScript | TypeScript</li>
            <li>Frameworks: Spring Boot | React.js | Node.js | Express | Next.js</li>
            <li>Full-Stack: MERN Stack | JWT/OAuth | RESTful APIs</li>
            <li>Backend: MVC | Middleware | Error Handling | DB Integration</li>
            <li>Frontend: Responsive UI | UX Optimization | State Management</li>
            <li>Other: OOP | Agile | Git | Debugging | API Security</li>
          </ul>
        </div>
        <img
          src="https://cdn.dribbble.com/users/1857592/screenshots/3848396/character-typing.gif"
          alt="Coding"
          className="w-80 rounded-lg shadow-lg"
        />
      </div>

      <div className="mb-10">
        <h3 className="text-2xl font-semibold mb-2">💻 Tech Stack:</h3>
        <div className="flex flex-wrap gap-4">
          {[
            'java',
            'python',
            'kotlinlang',
            'javascript',
            'react',
            'nodejs',
            'php',
            'html5',
            'css3',
            'mysql',
            'mongodb',
            'git',
            'figma',
            'linux',
            'arduino-1',
            'photoshop',
          ].map((tech, idx) => (
            <img
              key={idx}
              src={`https://raw.githubusercontent.com/devicons/devicon/master/icons/${tech}/${tech}-original.svg`}
              alt={tech}
              className="w-10 h-10"
              onError={(e) => {
                e.target.onerror = null;
                e.target.src = `https://www.vectorlogo.zone/logos/${tech}/${tech}-icon.svg`;
              }}
            />
          ))}
        </div>
      </div>

      <div className="mb-10">
        <h3 className="text-2xl font-semibold mb-4">🏆 GitHub Achievements:</h3>
        <img
          src="https://github-profile-trophy.vercel.app/?username=sevi2001&theme=gruvbox&row=1&column=6"
          alt="GitHub Trophies"
          className="mx-auto"
        />
      </div>

      <div className="mb-10">
        <h3 className="text-2xl font-semibold mb-4">📊 GitHub Stats:</h3>
        <div className="flex flex-col md:flex-row gap-6 justify-center items-center">
          <img
            src="https://github-readme-stats.vercel.app/api?username=sevi2001&show_icons=true&theme=radical"
            alt="GitHub Stats"
            className="w-full md:w-1/2"
          />
          <img
            src="https://github-readme-stats.vercel.app/api/top-langs/?username=sevi2001&layout=compact&theme=radical"
            alt="Top Languages"
            className="w-full md:w-1/2"
          />
        </div>
        <img
          src="https://github-readme-streak-stats.herokuapp.com/?user=sevi2001&theme=radical"
          alt="Streak Stats"
          className="mx-auto mt-6"
        />
      </div>

      <div className="mb-10">
        <h3 className="text-2xl font-semibold mb-2">🌐 Let's Connect:</h3>
        <div className="flex flex-wrap gap-4">
          {[
            {
              href: 'https://www.linkedin.com/in/sevindi-jayathilake/',
              label: 'LinkedIn',
              color: 'blue',
              logo: 'linkedin',
            },
            {
              href: 'https://www.instagram.com/sevi_jayathilake/',
              label: 'Instagram',
              color: 'E4405F',
              logo: 'instagram',
            },
            {
              href: 'https://www.facebook.com/sevindi.jayathilake',
              label: 'Facebook',
              color: '1877F2',
              logo: 'facebook',
            },
            {
              href: 'mailto:sevindijayathilake2001@gmail.com',
              label: 'Gmail',
              color: 'D14836',
              logo: 'gmail',
            },
          ].map(({ href, label, color, logo }, idx) => (
            <a key={idx} href={href} target="_blank" rel="noopener noreferrer">
              <img
                src={`https://img.shields.io/badge/${label}-${color}?style=for-the-badge&logo=${logo}&logoColor=white`}
                alt={label}
              />
            </a>
          ))}
        </div>
      </div>

      <div className="mb-10">
        <h3 className="text-2xl font-semibold mb-2">🚀 Featured Projects:</h3>
        <ul className="list-disc list-inside text-gray-300 space-y-2">
          <li>
            🔗 <a href="https://github.com/sevi2001/your-project" className="text-blue-400 underline">Project Name</a> – A brief description of your project
          </li>
          <li>
            🔗 <a href="https://github.com/sevi2001/another-project" className="text-blue-400 underline">Another Project</a> – Another cool thing you built
          </li>
        </ul>
      </div>

      <div className="text-center mt-10">
        <blockquote className="text-xl italic text-gray-400">
          "Code is like humor. When you have to explain it, it’s bad." – Cory House
        </blockquote>
        <div className="mt-4">
          <img
            src="https://komarev.com/ghpvc/?username=sevi2001&label=Profile%20views&color=0e75b6&style=flat"
            alt="Profile Views"
            className="mx-auto"
          />
        </div>
      </div>
    </div>
  );
};

export default Profile;
