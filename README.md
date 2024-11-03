import React from 'react';
import { Github, Twitter, Linkedin } from 'lucide-react';

const GithubProfile = () => {
  return (
    <div className="w-full max-w-4xl mx-auto text-center">
      {/* Header Wave */}
      <svg viewBox="0 0 1200 120" className="w-full h-24">
        <path
          d="M0,0 L1200,0 L1200,120 Q900,80 600,120 Q300,160 0,120 Z"
          fill="url(#gradient)"
        >
          <defs>
            <linearGradient id="gradient" x1="0%" y1="0%" x2="100%" y2="0%">
              <stop offset="0%" style={{ stopColor: '#FF1493' }} />
              <stop offset="100%" style={{ stopColor: '#FF69B4' }} />
            </linearGradient>
          </defs>
        </path>
      </svg>

      {/* Name Section */}
      <div className="text-4xl font-bold mb-4 bg-gradient-to-r from-pink-500 to-purple-500 text-transparent bg-clip-text">
        Rodolfo Chivalan
      </div>

      {/* Title Section */}
      <div className="text-2xl mb-8 text-pink-500">
        System Engineering Student
      </div>

      {/* Social Icons */}
      <div className="flex justify-center gap-8 mb-8">
        <Linkedin size={32} className="text-pink-500 hover:text-pink-600 cursor-pointer" />
        <Twitter size={32} className="text-pink-500 hover:text-pink-600 cursor-pointer" />
        <Github size={32} className="text-pink-500 hover:text-pink-600 cursor-pointer" />
      </div>

      {/* Stats Section */}
      <h2 className="text-2xl font-bold mb-4">📊 GitHub Stats</h2>
      
      {/* GitHub Stats Cards */}
      <div className="space-y-4">
        {/* Main Stats Card */}
        <div className="bg-gray-900 rounded-lg p-4 mx-auto max-w-2xl">
          <div className="grid grid-cols-3 gap-4">
            <div className="text-center">
              <div className="text-2xl font-bold text-pink-500">150+</div>
              <div className="text-sm text-gray-400">Contributions</div>
            </div>
            <div className="text-center">
              <div className="text-2xl font-bold text-pink-500">10+</div>
              <div className="text-sm text-gray-400">Repositories</div>
            </div>
            <div className="text-center">
              <div className="text-2xl font-bold text-pink-500">5+</div>
              <div className="text-sm text-gray-400">Projects</div>
            </div>
          </div>
        </div>

        {/* Streak Stats Card */}
        <div className="bg-gray-900 rounded-lg p-4 mx-auto max-w-2xl">
          <div className="h-4 w-full bg-gray-800 rounded">
            <div className="h-full w-3/4 bg-gradient-to-r from-pink-500 to-purple-500 rounded"></div>
          </div>
          <div className="mt-2 text-sm text-gray-400">Current Streak: 7 days</div>
        </div>

        {/* Languages Card */}
        <div className="bg-gray-900 rounded-lg p-4 mx-auto max-w-2xl">
          <div className="grid grid-cols-2 gap-2">
            <div className="text-sm text-gray-400">JavaScript</div>
            <div className="h-2 bg-gray-800 rounded">
              <div className="h-full w-3/4 bg-yellow-400 rounded"></div>
            </div>
            <div className="text-sm text-gray-400">Python</div>
            <div className="h-2 bg-gray-800 rounded">
              <div className="h-full w-1/2 bg-blue-500 rounded"></div>
            </div>
            <div className="text-sm text-gray-400">HTML/CSS</div>
            <div className="h-2 bg-gray-800 rounded">
              <div className="h-full w-2/3 bg-orange-500 rounded"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  );
};

export default GithubProfile;
