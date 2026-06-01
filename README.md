# RSL Bank Specification

## Project Description

This project contains a formal specification of a simplified banking system written in **RSL** — the RAISE Specification Language.

The project is not a full executable banking application. Its purpose is to formally describe the structure and behavior of a bank system using abstract data types, functions, invariants, preconditions, and postconditions.

## Task

The task is to specify a bank system that contains:

* a list of users;
* a list of accounts for each user;
* different account types:

  * current accounts;
  * deposits;
  * credits;
* additional information for deposits and credits, such as:

  * interest rate;
  * term;
  * replenishment availability;
  * capitalization for deposits;
  * credit limit for credits;
* an operation for replenishing an account;
* an operation for transferring money from one account to another.

## About RSL

**RSL** stands for **RAISE Specification Language**. It is a formal specification language used to describe software systems at an abstract mathematical level.

Unlike common programming languages, RSL is mainly used to describe what a system must do, rather than how it should be implemented. It allows defining:

* data types;
* system states;
* functions;
* invariants;
* preconditions;
* postconditions.

This makes RSL useful for formal reasoning about system correctness before implementation.

## System Scope

The specification models a simplified bank system. The main system state is represented by the `Bank` type, which contains a list of users. Each user has a unique identifier and a list of accounts. Each account has an identifier, a balance, and an account type.

The following functionality is included:

* checking whether an account type is valid;
* checking whether an account can be replenished;
* checking whether a user exists;
* checking whether an account exists;
* finding an account by its identifier;
* checking uniqueness of users and accounts;
* checking whether the bank state is well-formed;
* replenishing an account;
* transferring money between accounts.

## Result

The result of this project is a formal RSL specification of a simplified bank system. The specification defines the system structure, correctness conditions, and the behavior of the two main banking operations: account replenishment and money transfer.
