syntax = "proto3";

package portfolio;

message Portfolio {
  string full_name = 1;
  string email = 2;
  string course = 3;
  string college = 4;
  string summary = 5;
  repeated string achievements = 6;
  repeated string skills = 7;
  string github_url = 8;
  repeated Project projects = 9;
  repeated string certifications = 10;
}

message Project {
  string title = 1;
  string description = 2;
  string github_link = 3;
}

message Example {
  Portfolio eniya_portfolio = 1;
}

// Example data (for reference)
Portfolio eniya_portfolio = {
  full_name: "Eniya Eni"
  email: "eniya7665@gmail.com"
  course: "B.Tech Cyber Security"
  college: "Mahendra Engineering College"
  summary: "Passionate cybersecurity student focused on ethical hacking and digital defense."
  achievements: ["Won 2nd place in National Expo 2025"]
  skills: ["Python", "Linux", "Networking", "Ethical Hacking", "Git"]
  github_url: "https://github.com/eniya7665"
  projects: [
    { title: "SecureNet Analyzer", description: "Network vulnerability scanner.", github_link: "https://github.com/eniya7665/SecureNet-Analyzer" },
    { title: "PhishGuard", description: "Phishing detection using ML.", github_link: "https://github.com/eniya7665/PhishGuard" }
  ]
  certifications: ["CEH (in progress)"]
};# Eniya
