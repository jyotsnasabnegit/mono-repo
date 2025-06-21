# mono-repo
 
Steps:
1. Install pnpm : npm -g intall pnpm
2. pnpm init
3. Create pnpm-workspace.yaml
Add : 
packages: 
 - "packages/*"
 - "apps/*"
4. Create apps under apps/
pnpm create vite apps/<name_of_app>
cd apps/<name_of_app>
pnpm install
5. Run app
pnpm --filter restaurant-mgmt-admin dev
6. In root package.json, add script
"start:ui": "pnpm --filter <name_of_app> dev"


