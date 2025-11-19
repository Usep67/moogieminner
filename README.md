import React from "react";

// Single-file React component styled with Tailwind CSS.
// Default export: <MoogieMinner />
// Usage: place inside a React app with Tailwind configured.

export default function MoogieMinner() {
  return (
    <div className="min-h-screen bg-gradient-to-b from-slate-900 via-slate-800 to-slate-900 text-slate-100 flex items-center justify-center p-6">
      <div className="max-w-5xl w-full grid grid-cols-1 lg:grid-cols-3 gap-8 items-center">
        {/* Left: Header + description */}
        <header className="lg:col-span-1 flex flex-col gap-6">
          <div>
            <h1 className="text-4xl md:text-5xl font-extrabold tracking-tight">Moogie Minner</h1>
            <p className="mt-2 text-slate-300">Limited edition Moogie NFT collection — playful, pixel-perfect creatures ready for minting.</p>
          </div>

          <div className="mt-4 p-4 rounded-2xl bg-white/5 border border-white/6 shadow-lg">
            <h2 className="text-sm uppercase text-slate-300 tracking-wider">Collection</h2>
            <p className="mt-1 text-lg font-medium">Moogie NFT</p>

            <div className="mt-4 grid grid-cols-2 gap-3">
              <div className="p-3 rounded-xl bg-white/3">
                <div className="text-xs text-slate-300">Number of NFTs available</div>
                <div className="mt-1 text-xl font-semibold">10,000</div>
              </div>

              <div className="p-3 rounded-xl bg-white/3">
                <div className="text-xs text-slate-300">Price per NFT</div>
                <div className="mt-1 text-xl font-semibold">0.0003 ETH</div>
              </div>
            </div>

            <div className="mt-5">
              <button
                className="w-full flex items-center justify-center gap-3 py-3 rounded-xl bg-gradient-to-r from-emerald-400 to-teal-400 text-slate-900 font-semibold shadow-2xl transform hover:scale-[1.01] active:scale-[0.99]"
                aria-label="Mint a Moogie"
              >
                <svg xmlns="http://www.w3.org/2000/svg" className="h-5 w-5" viewBox="0 0 20 20" fill="currentColor" aria-hidden>
                  <path fillRule="evenodd" d="M10 5a1 1 0 011 1v3h3a1 1 0 110 2h-3v3a1 1 0 11-2 0v-3H6a1 1 0 110-2h3V6a1 1 0 011-1z" clipRule="evenodd" />
                </svg>
                <span>Mint</span>
              </button>

              <div className="mt-3 text-xs text-slate-400">Press the <span className="font-semibold">+ Mint</span> button to mint your Moogie.</div>
            </div>
          </div>
        </header>

        {/* Center: Large image */}
        <div className="lg:col-span-1 flex items-center justify-center">
          <div className="relative w-full max-w-md aspect-square rounded-3xl overflow-hidden border-2 border-white/5 bg-gradient-to-br from-indigo-700 to-fuchsia-600 shadow-2xl">
            {/* Replace the src below with the actual Moogie NFT image URL */}
            <img
              src="https://via.placeholder.com/800x800.png?text=Moogie+NFT"
              alt="Moogie NFT"
              className="object-cover w-full h-full"
            />

            <div className="absolute left-3 bottom-3 bg-black/40 backdrop-blur rounded-full px-3 py-1 text-xs text-white/90">
              Moogie NFT
            </div>
          </div>
        </div>

        {/* Right: Additional actions / stats */}
        <aside className="lg:col-span-1 flex flex-col gap-6">
          <div className="p-4 rounded-2xl bg-white/5 border border-white/6">
            <h3 className="text-sm text-slate-300 uppercase tracking-wide">Mint progress</h3>
            <div className="mt-3">
              {/* Example progress bar (static). You can wire this up to real state. */}
              <div className="w-full bg-white/6 rounded-full h-3 overflow-hidden">
                <div className="h-3 rounded-full" style={{ width: '28%', background: 'linear-gradient(90deg,#10b981,#06b6d4)' }} />
              </div>

              <div className="mt-2 text-xs text-slate-400">2,800 / 10,000 minted</div>
            </div>
          </div>

          <div className="p-4 rounded-2xl bg-white/5 border border-white/6 flex flex-col gap-3">
            <div className="text-sm text-slate-300 uppercase tracking-wide">Quick actions</div>
            <button className="py-2 rounded-lg bg-white/3 text-sm font-medium">View Collection</button>
            <button className="py-2 rounded-lg bg-white/3 text-sm font-medium">Contract</button>
            <button className="py-2 rounded-lg bg-white/3 text-sm font-medium">Twitter</button>
          </div>
        </aside>
      </div>
    </div>
  );
}
