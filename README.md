Rewrd – Loyalty & Cashback Platform (Architecture Case Study)
Overview

Rewrd is a full-stack loyalty and cashback platform that enables businesses to reward customers for repeat purchases using points, store credit, or cashback. The platform is designed to improve customer retention for merchants while providing users with tangible value for everyday spending.

This repository is a public architecture and system design case study. The production codebase is private.

Problem Statement

Small and mid-sized businesses often struggle with customer retention. Traditional discounts are short-term, difficult to track, and do not incentivize long-term loyalty. Businesses need a system that:

Encourages repeat purchases

Is easy for customers to understand and use

Provides merchants with visibility into customer engagement

Scales as transaction volume increases

Rewrd was built to solve these challenges by introducing a structured, automated loyalty and cashback system.

Solution

Rewrd provides:

A customer-facing web application where users earn and redeem rewards

A merchant dashboard for managing loyalty programs

A backend system that reliably tracks transactions, rewards, and redemptions

The platform prioritizes performance, reliability, and clear reward flows to ensure trust and usability for both customers and businesses.

My Role

I led the design and delivery of the Rewrd platform, owning the product end-to-end while collaborating with other engineers on backend implementation.

My responsibilities included:

Product design and overall system architecture

Frontend development and user experience implementation

Backend feature development and API design (in collaboration with backend engineers)

Database schema design and data flow modeling

Aligning architectural decisions, reviewing backend contributions, and ensuring system consistency

Deployment, CI/CD setup, and production maintenance

This role required balancing hands-on development with technical leadership and cross-team collaboration.

System Architecture
High-Level Architecture

Frontend: React (owned and implemented by me)

Backend: Node.js (REST APIs, built collaboratively)

Database: Relational database (users, transactions, rewards)

Caching: Redis (used for performance optimization and reduced database load)

Deployment: Cloud-hosted with CI/CD pipelines for automated builds and deployments

The architecture follows a modular, service-oriented approach to ensure scalability, maintainability, and clear ownership boundaries across the team.

Core Features
User Features

User registration and authentication

Reward accrual based on eligible purchases

Reward balance tracking

Reward redemption flow

Merchant Features

Business onboarding

Loyalty program configuration

Customer engagement tracking

Reward issuance and monitoring

Key Engineering Decisions
1. Modular Backend Design

The backend is structured into clearly separated modules (authentication, rewards, transactions, users), enabling independent development, testing, and scaling of features.

2. Performance Optimization

Implemented caching for frequently accessed user and reward data

Optimized database queries to reduce latency

Designed APIs to support concurrent user activity

3. Data Consistency & Reliability

Reward calculations are handled server-side to prevent manipulation and ensure accurate balances. Transactions are validated before rewards are issued to maintain system integrity.

4. Scalability Considerations

The system was designed to support increased transaction volume by:

Allowing horizontal scaling of backend services

Using caching to minimize database load

Keeping reward logic stateless where possible

Challenges & Trade-offs

Balancing real-time reward updates with overall system performance

Designing reward logic flexible enough to support different merchant requirements

Prioritizing correctness and reliability over premature optimization

Impact

Enabled businesses to run structured loyalty programs without building custom systems

Improved customer retention through tangible reward incentives

Established a scalable foundation for future features such as advanced analytics and expanded cashback integrations

Supported collaborative backend development while maintaining architectural consistency and performance standards

Tech Stack

React

Node.js

REST APIs

PostgreSQL / MySQL

Redis

Git & CI/CD

Notes

This repository intentionally excludes production source code. Its purpose is to demonstrate system design thinking, architectural decisions, and real-world problem solving behind a production-grade fintech product.

Contact

Princess Jewel Jel-Edema
Senior Full Stack Engineer (React & Node.js)
Portfolio: https://princess-jewel.vercel.app
LinkedIn: https://linkedin.com/in/princess-jewel-jel-edema
