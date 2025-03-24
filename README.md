import React from 'react';
import { Shield, Bell, Menu, ArrowRight, CheckCircle, Clock, AlertTriangle } from 'lucide-react';

const UniqueDashboardUI = () => {
  return (
    <div className="min-h-screen bg-neutral-50 text-neutral-800">
      {/* Top Bar */}
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
      
      {/* Left Action Bar */}
      <div className="fixed left-6 top-24 bottom-6 w-12 flex flex-col items-center space-y-4 z-10">
        <button className="h-12 w-12 rounded-full bg-emerald-500 text-white shadow-md flex items-center justify-center">
          <span className="text-xl font-bold">62</span>
        </button>
        
        <div className="h-32 w-0.5 bg-neutral-200 my-2"></div>
        
        <button className="h-10 w-10 rounded-full bg-white shadow-sm text-neutral-800 flex items-center justify-center hover:shadow-md">
          <Menu className="h-5 w-5" />
        </button>
      </div>
      
      {/* Main Content */}
      <main className="pt-28 pl-24 pr-6 pb-12">
        <div className="max-w-6xl mx-auto">
          {/* Header */}
          <div className="mb-12">
            <h1 className="text-3xl font-light mb-1">Good afternoon, <span className="font-semibold">Juan</span></h1>
            <p className="text-neutral-500">Your security score is <span className="text-emerald-500 font-medium">62</span> — moderate protection</p>
          </div>
          
          {/* Content Grid */}
          <div className="space-y-12">
            {/* Priorities Section */}
            <section>
              <h2 className="text-lg font-semibold mb-8 pl-1 border-l-4 border-emerald-500 pl-4">Critical Priorities</h2>
              
              <div className="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <div className="bg-white rounded-lg shadow-sm hover:shadow-md transition-shadow">
                  <div className="py-5 px-6 border-b border-neutral-100 flex justify-between items-center">
                    <h3 className="font-medium">Enable Two-Factor Authentication</h3>
                    <span className="inline-block px-2.5 py-1 bg-red-100 text-red-700 text-xs rounded-full">Critical</span>
                  </div>
                  <div className="p-6">
                    <div className="mb-5">
                      <p className="text-neutral-600">Secure your accounts with an additional layer of protection beyond passwords.</p>
                    </div>
                    <div className="flex justify-between items-center text-sm">
                      <div className="flex items-center">
                        <div className="w-9 h-9 rounded-full bg-red-100 flex items-center justify-center mr-3">
                          <AlertTriangle className="w-4 h-4 text-red-600" />
                        </div>
                        <span className="text-neutral-500">Data Privacy Act Requirement</span>
                      </div>
                      <button className="text-emerald-600 hover:text-emerald-700 font-medium flex items-center">
                        Implement
                        <ArrowRight className="w-4 h-4 ml-1" />
                      </button>
                    </div>
                  </div>
                </div>
                
                <div className="bg-white rounded-lg shadow-sm hover:shadow-md transition-shadow">
                  <div className="py-5 px-6 border-b border-neutral-100 flex justify-between items-center">
                    <h3 className="font-medium">Update All Software and Systems</h3>
                    <span className="inline-block px-2.5 py-1 bg-red-100 text-red-700 text-xs rounded-full">Critical</span>
                  </div>
                  <div className="p-6">
                    <div className="mb-5">
                      <p className="text-neutral-600">Install the latest security patches to protect against known vulnerabilities.</p>
                    </div>
                    <div className="flex justify-between items-center text-sm">
                      <div className="flex items-center">
                        <div className="w-9 h-9 rounded-full bg-red-100 flex items-center justify-center mr-3">
                          <AlertTriangle className="w-4 h-4 text-red-600" />
                        </div>
                        <span className="text-neutral-500">Basic Security</span>
                      </div>
                      <button className="text-emerald-600 hover:text-emerald-700 font-medium flex items-center">
                        Implement
                        <ArrowRight className="w-4 h-4 ml-1" />
                      </button>
                    </div>
                  </div>
                </div>
              </div>
            </section>
            
            {/* Security Metrics */}
            <section>
              <h2 className="text-lg font-semibold mb-8 pl-1 border-l-4 border-emerald-500 pl-4">Security Status</h2>
              
              <div>
                {/* Domain Bars */}
                <div className="space-y-6 mb-6">
                  <div>
                    <div className="flex justify-between items-center mb-2">
                      <div className="flex items-center">
                        <div className="w-3 h-3 rounded-full bg-emerald-500 mr-3"></div>
                        <span className="font-medium">Data Protection</span>
                      </div>
                      <div className="flex items-center">
                        <span className="text-neutral-800 font-medium">80</span>
                        <span className="text-neutral-400 text-sm ml-1">/100</span>
                      </div>
                    </div>
                    <div className="h-2 bg-neutral-100 rounded-full w-full overflow-hidden">
                      <div className="h-2 bg-emerald-500 rounded-full" style={{ width: '80%' }}></div>
                    </div>
                  </div>
                  
                  <div>
                    <div className="flex justify-between items-center mb-2">
                      <div className="flex items-center">
                        <div className="w-3 h-3 rounded-full bg-red-500 mr-3"></div>
                        <span className="font-medium">Network Security</span>
                      </div>
                      <div className="flex items-center">
                        <span className="text-neutral-800 font-medium">45</span>
                        <span className="text-neutral-400 text-sm ml-1">/100</span>
                      </div>
                    </div>
                    <div className="h-2 bg-neutral-100 rounded-full w-full overflow-hidden">
                      <div className="h-2 bg-red-500 rounded-full" style={{ width: '45%' }}></div>
                    </div>
                  </div>
                  
                  <div>
                    <div className="flex justify-between items-center mb-2">
                      <div className="flex items-center">
                        <div className="w-3 h-3 rounded-full bg-amber-500 mr-3"></div>
                        <span className="font-medium">Employee Awareness</span>
                      </div>
                      <div className="flex items-center">
                        <span className="text-neutral-800 font-medium">60</span>
                        <span className="text-neutral-400 text-sm ml-1">/100</span>
                      </div>
                    </div>
                    <div className="h-2 bg-neutral-100 rounded-full w-full overflow-hidden">
                      <div className="h-2 bg-amber-500 rounded-full" style={{ width: '60%' }}></div>
                    </div>
                  </div>
                  
                  <div>
                    <div className="flex justify-between items-center mb-2">
                      <div className="flex items-center">
                        <div className="w-3 h-3 rounded-full bg-blue-500 mr-3"></div>
                        <span className="font-medium">Incident Response</span>
                      </div>
                      <div className="flex items-center">
                        <span className="text-neutral-800 font-medium">70</span>
                        <span className="text-neutral-400 text-sm ml-1">/100</span>
                      </div>
                    </div>
                    <div className="h-2 bg-neutral-100 rounded-full w-full overflow-hidden">
                      <div className="h-2 bg-blue-500 rounded-full" style={{ width: '70%' }}></div>
                    </div>
                  </div>
                </div>
                
                {/* Task Completion */}
                <div className="bg-white rounded-lg shadow-sm p-6">
                  <div className="flex justify-between items-center mb-6">
                    <h3 className="font-medium">Task Completion</h3>
                    <span className="text-neutral-500 text-sm">8 of 20 completed</span>
                  </div>
                  
                  <div className="w-full h-2 bg-neutral-100 rounded-full overflow-hidden mb-6">
                    <div className="h-2 bg-emerald-500 rounded-full" style={{ width: '40%' }}></div>
                  </div>
                  
                  <div className="grid grid-cols-1 md:grid-cols-3 gap-4 text-sm">
                    <div className="flex items-center justify-center p-3 bg-neutral-50 rounded-lg">
                      <div className="w-7 h-7 rounded-full bg-emerald-100 flex items-center justify-center mr-2">
                        <CheckCircle className="w-4 h-4 text-emerald-600" />
                      </div>
                      <span className="text-neutral-600">8 Completed</span>
                    </div>
                    
                    <div className="flex items-center justify-center p-3 bg-neutral-50 rounded-lg">
                      <div className="w-7 h-7 rounded-full bg-amber-100 flex items-center justify-center mr-2">
                        <Clock className="w-4 h-4 text-amber-600" />
                      </div>
                      <span className="text-neutral-600">3 In Progress</span>
                    </div>
                    
                    <div className="flex items-center justify-center p-3 bg-neutral-50 rounded-lg">
                      <div className="w-7 h-7 rounded-full bg-neutral-200 flex items-center justify-center mr-2">
                        <AlertTriangle className="w-4 h-4 text-neutral-600" />
                      </div>
                      <span className="text-neutral-600">9 Not Started</span>
                    </div>
                  </div>
                </div>
              </div>
            </section>
            
            {/* Resources */}
            <section>
              <h2 className="text-lg font-semibold mb-8 pl-1 border-l-4 border-emerald-500 pl-4">Educational Resources</h2>
              
              <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
                {Array.from({ length: 3 }).map((_, i) => (
                  <div key={i} className="group relative">
                    <div className="absolute -inset-0.5 bg-gradient-to-r from-emerald-500 to-emerald-300 rounded-lg blur opacity-0 group-hover:opacity-100 transition duration-500"></div>
                    <div className="relative bg-white rounded-lg shadow-sm p-6 h-full flex flex-col">
                      <h3 className="font-medium mb-2">
                        {i === 0 && "Data Privacy Act Guide"}
                        {i === 1 && "Password Best Practices"}
                        {i === 2 && "Employee Training Template"}
                      </h3>
                      <p className="text-sm text-neutral-600 mb-4 flex-grow">
                        {i === 0 && "Simple explanation of compliance requirements for Filipino businesses."}
                        {i === 1 && "How to create and manage secure passwords for your business accounts."}
                        {i === 2 && "Simple training materials for your team to learn cybersecurity basics."}
                      </p>
                      <div className="flex items-center justify-between mt-2 text-sm">
                        <span className="text-neutral-500">
                          {i === 0 && "5 min read"}
                          {i === 1 && "4 min read"}
                          {i === 2 && "PDF Template"}
                        </span>
                        <button className="text-emerald-600 hover:text-emerald-700 font-medium">
                          {i === 2 ? "Download" : "View"}
                        </button>
                      </div>
                    </div>
                  </div>
                ))}
              </div>
            </section>
            
            {/* Next Assessment */}
            <section className="flex items-center justify-between bg-white rounded-lg shadow-sm p-6">
              <div>
                <h2 className="text-lg font-semibold mb-1">Next Assessment: May 5, 2025</h2>
                <p className="text-neutral-500">15 days remaining until your quarterly security review</p>
              </div>
              <button className="px-5 py-2.5 bg-emerald-500 text-white rounded-lg hover:bg-emerald-600 transition-colors">
                Start Early
              </button>
            </section>
          </div>
        </div>
      </main>
    </div>
  );
};

export default UniqueDashboardUI;
