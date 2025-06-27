import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Github, Linkedin, Mail } from "lucide-react";

export default function Portfolio() {
  return (
    <div className="min-h-screen bg-gray-100 p-6">
      <div className="max-w-4xl mx-auto space-y-10">
        <header className="text-center">
          <h1 className="text-4xl font-bold">Hi, I'm Arpit Srivastava</h1>
          <p className="text-xl text-gray-600 mt-2">IT Student | Web Developer | Video Editor</p>
          <div className="flex justify-center space-x-4 mt-4">
            <a href="https://github.com/Arpit-code24" target="_blank"><Github /></a>
            <a href="https://www.linkedin.com/in/arpit-srivastava-509199265" target="_blank"><Linkedin /></a>
            <a href="mailto:arpitpersonal1805@gmail.com"><Mail /></a>
          </div>
        </header>

        <section>
          <h2 className="text-2xl font-semibold mb-4">About Me</h2>
          <Card>
            <CardContent className="p-4 text-gray-700">
              I'm a 3rd year IT student with a passion for web development and video editing. I enjoy building clean, functional websites and creating engaging visual content. Currently, I'm looking for opportunities to grow through internships and freelance work.
            </CardContent>
          </Card>
        </section>

        <section>
          <h2 className="text-2xl font-semibold mb-4">Projects</h2>
          <div className="grid md:grid-cols-2 gap-4">
            <Card>
              <CardContent className="p-4">
                <h3 className="text-xl font-semibold">Personal Portfolio</h3>
                <p className="text-gray-600">A responsive portfolio website built with React and Tailwind CSS.</p>
              </CardContent>
            </Card>
            <Card>
              <CardContent className="p-4">
                <h3 className="text-xl font-semibold">Event Highlights Reel</h3>
                <p className="text-gray-600">Edited promotional videos for an event management company using Premiere Pro.</p>
              </CardContent>
            </Card>
            <Card>
              <CardContent className="p-4">
                <h3 className="text-xl font-semibold">Direct Market Access Platform</h3>
                <p className="text-gray-600">Developed a web platform to connect farmers directly with consumers, eliminating middlemen and enabling fair trade.</p>
              </CardContent>
            </Card>
            <Card>
              <CardContent className="p-4">
                <h3 className="text-xl font-semibold">Social Media & Video Editor – JINEE EVENTS, Lucknow</h3>
                <p className="text-gray-600">Handled video editing and social media content creation for <a href="https://www.instagram.com/jinee_events?utm_source=ig_web_button_share_sheet&igsh=Y3hpcjJ4Z2M2bmR6" className="text-blue-600 underline" target="_blank">JINEE EVENTS</a>, contributing to event promotions and audience engagement.</p>
              </CardContent>
            </Card>
          </div>
        </section>

        <section>
          <h2 className="text-2xl font-semibold mb-4">Skills</h2>
          <Card>
            <CardContent className="p-4 grid grid-cols-2 gap-2 text-gray-700">
              <span>HTML/CSS</span>
              <span>JavaScript</span>
              <span>React</span>
              <span>Tailwind CSS</span>
              <span>Java</span>
              <span>SQL</span>
            </CardContent>
          </Card>
        </section>

        <section className="text-center">
          <h2 className="text-2xl font-semibold mb-4">Let's Connect</h2>
          <p className="mb-4">I'm open to internships, freelance projects, and collaborations.</p>
          <Button asChild>
            <a href="mailto:arpitpersonal1805@gmail.com">Get in Touch</a>
          </Button>
        </section>
      </div>
    </div>
  );
}
