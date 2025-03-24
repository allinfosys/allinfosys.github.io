<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>React on GitHub Pages</title>
    <script src="https://unpkg.com/react@18/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/lucide-react@latest"></script>
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-100">

    <div id="root"></div> <!-- React will render here -->

    <script type="text/babel">
        const { useState } = React;
        const { createRoot } = ReactDOM;
        const { Shield, Bell, Menu, ArrowRight, CheckCircle, Clock, AlertTriangle } = lucideReact;

        function UniqueDashboardUI() {
            return (
                <div className="min-h-screen bg-neutral-50 text-neutral-800">
                    <div className="fixed top-0 left-0 right-0 h-16 bg-white flex items-center justify-between px-6 z-10 border-b border-neutral-100">
                        <div className="flex items-center space-x-3">
                            <div className="h-8 w-8 rounded-md bg-emerald-500 flex items-center justify-center shadow-sm">
                                <Shield className="h-5 w-5 text-white" />
                            </div>
                            <span className="font-semibold text-lg">SecureMe</span>
                        </div>
                        <div className="flex items-center space-x-4">
                            <button className="h-9 w-9 flex items-center justify-center rounded-full hover:bg-neutral-100">
                                <Bell className="h-5 w-5 text-neutral-600" />
                            </button>
                            <div className="h-9 w-9 bg-neutral-200 rounded-full flex items-center justify-center">
                                <span className="text-sm font-medium">JS</span>
                            </div>
                        </div>
                    </div>

                    <main className="pt-28 pl-24 pr-6 pb-12">
                        <div className="max-w-6xl mx-auto">
                            <h1 className="text-3xl font-light mb-1">Good afternoon, <span className="font-semibold">Juan</span></h1>
                            <p className="text-neutral-500">Your security score is <span className="text-emerald-500 font-medium">62</span> — moderate protection</p>
                        </div>
                    </main>
                </div>
            );
        }

        const root = createRoot(document.getElementById("root"));
        root.render(<UniqueDashboardUI />);
    </script>

</body>
</html>
