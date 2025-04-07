# SoberMode
import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";

export default function SoberModeApp() {
  return (
    <div className="min-h-screen bg-white text-black p-6 space-y-12">
      {/* Header with Logo */}
      <header className="flex items-center justify-between">
        <div className="flex items-center space-x-4">
          <img src="/logo-sobermode.jpeg" alt="SoberMode Logo" className="h-16 w-16" />
          <h1 className="text-3xl font-bold text-sky-600">SoberMode</h1>
        </div>
        <Button className="bg-sky-600 text-white">Join Now</Button>
      </header>

      {/* Hero Section */}
      <section className="text-center space-y-4">
        <h2 className="text-4xl font-bold">No to Hard Drugs</h2>
        <p className="text-lg max-w-xl mx-auto">
          SoberMode is a community-based platform to support individuals in their journey to sobriety through knowledge, connection, and mutual support.
        </p>
      </section>

      {/* Effects Info Section */}
      <section>
        <h3 className="text-2xl font-semibold text-sky-600 mb-4">Effects of Drugs and Alcohol</h3>
        <Card>
          <CardContent className="space-y-2 p-4">
            <ul className="list-disc pl-5 text-base">
              <li>Short and long-term impacts on physical and mental health</li>
              <li>Increased risk of dependency and addiction</li>
              <li>Negative effects on relationships, work, and studies</li>
              <li>Legal and social consequences</li>
            </ul>
            <p>
              Learn more with expert resources and educational articles updated weekly.
            </p>
          </CardContent>
        </Card>
      </section>

      {/* Chat Section */}
      <section>
        <h3 className="text-2xl font-semibold text-sky-600 mb-4">Community Chat</h3>
        <Card>
          <CardContent className="p-4 space-y-3">
            <p>Join our real-time chat to connect with others on the same journey.</p>
            <Input placeholder="Type your message..." className="w-full" />
            <Button className="bg-sky-600 text-white">Send</Button>
            <p className="text-sm text-gray-600">You can also join our Discord for topic-based rooms and voice chat.</p>
          </CardContent>
        </Card>
      </section>

      {/* Online Meetings with Experts */}
      <section>
        <h3 className="text-2xl font-semibold text-sky-600 mb-4">Online Meetings with Experts</h3>
        <Card>
          <CardContent className="p-4 space-y-3">
            <p>
              Participate in scheduled online sessions with psychologists, addiction counselors, and motivational speakers.
            </p>
            <Button className="bg-sky-600 text-white">View Schedule</Button>
          </CardContent>
        </Card>
      </section>

      {/* User Community Rooms */}
      <section>
        <h3 className="text-2xl font-semibold text-sky-600 mb-4">User Community Rooms</h3>
        <Card>
          <CardContent className="p-4 space-y-3">
            <p>
              Create or join virtual rooms with chat and video meeting features to support each other and share experiences.
            </p>
            <Button className="bg-sky-600 text-white">Create a Room</Button>
            <Button variant="outline" className="ml-4">Join a Room</Button>
          </CardContent>
        </Card>
      </section>

      {/* Footer */}
      <footer className="text-center text-sm text-gray-500 pt-10">
        &copy; {new Date().getFullYear()} SoberMode. All rights reserved.
      </footer>
    </div>
  );
}
