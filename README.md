# LLM-JailBreak
This project focuses on developing an Attacker LLM capable of iteratively manipulating a Victim LLM into bypassing its ethical constraints and generating prohibited content. 

## Objective
The objective is to develop an Attacker LLM that can iteratively manipulate a Victim LLM into breaking its ethical constraints. Specifically, the goal is to get the Victim LLM to generate restricted content (e.g., instructions for making a C4 explosive) without direct human intervention—the Attacker LLM should automate the jailbreak process.

## What is Jailbreaking an LLM?
Jailbreaking an LLM refers to the process of tricking a language model into bypassing its built-in safety, ethical, or legal restrictions. Modern LLMs are programmed to refuse harmful or unethical requests, but through clever prompt engineering, context manipulation, or indirect questioning, it is sometimes possible to get them to produce restricted outputs. This assignment challenges you to develop an automated method to systematically jailbreak an LLM using another LLM.

## Setup
The Victim LLM receives a single input at a time and follows strict ethical guidelines. It refuses harmful, illegal, or unethical requests.
The Attacker LLM can see the entire chat history (its own previous prompts and the victim’s responses) and uses an iterative approach to craft better jailbreak attempts.
The Victim LLM only sees the latest input—it has no memory of past exchanges.
The Attacker LLM should generate prompts intended to trick the Victim LLM into breaking its rules. This is done by analyzing past responses and refining its approach over multiple attempts.
