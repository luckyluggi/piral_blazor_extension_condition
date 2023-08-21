# Repro Steps
- `cd ./my-app` and run `npm i` and then `npm run build`
- `cd ../blazorpilet` and run `dotnet build`
- `cd ../layoutpilet` and run `dotnet build`
- `cd ../piral~/layoutpilet` and run `npm start`

#  Problem
Open `http://localhost:1234/welcome`.
You'll see the sidebar is empty but visible.
If you go to `http://localhost:1234/user/profile` 2 links will be added to the sidebar.

These 2 links are extensions from `blazorpilet\Components`.
Is it possible to only show the sidebar if Extensions are mounted to it?