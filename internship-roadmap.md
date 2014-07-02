# Internship Roadmap

* Intern Name Rahul Gopinath
* Hiring Manager Michelle Johansen
* Department ENG/Platform
* Start Date 6/30/2014
* Buddy Kylo Ginsberg
* End Date 9/26/2014

## Scorecard
Engineering Scorecard can be found here
 
## Internship Summary / Scope of Work 
Platform Client internship. Rahul will spend the internship embedded with 
the Platform Client team, acting essentially in the same capacity as a 
full-time Engineer. He will focus on Ruby-based static analysis and code 
factoring in the Puppet project, and also be exposed to C++ work in the Native 
Facter project.


__This work will give him an opportunity to learn__

* Our agile workflow, including daily standups, weekly planning, etc
* The lifecycle of a ticket: development, code review, commit, CI, functional review
* Static analysis tools for Ruby
* C++11 tooling
* Code refactoring and test development
* Tools for working cross-platform: vcloud, vagrant, docker
* Managing branches with git and developer-centric release mechanics

## Key Objectives

1. Become familiar with the agile workflow and ticket lifecycle.
2. Static Analysis of Puppet Ruby code
3. Refactoring of Puppet Modules
4. Native Facter support for Solaris
5. Work with community contributions.
6. Release software

### Key Objective #1 (from above)
 Become familiar with the agile workflow and ticket lifecycle.

Point Person(s): Kylo Ginsberg

| Tasks / Milestones | Milestone |
|--------------------|----------|
| Agile orientation | Attend daily startups, weekly planning, and biweekly retrospective.
| Ticket lifecycle | Review platform board. Try the No Team / Client Team filters. Add a component to a currently No Team ticket so that it's (correctly) Client Team. Move a ticket between columns (then move it back so no one's confused).
| Jenkins orientation | Manually start a puppet spec job, review logs after it completes. Ditto for an acceptance job. 
| VM orientation | Install puppet on a vcloud vm, on a vagrant vm.  
| Ruby orientation | Break puppet in some random way, run rspec to verify it’s broken, fix it, verify with rspec. No commits! 

#### Key Resources (people, departments, links, etc.)
N.A
 
### Key Objective #2 (from above)
 Static Analysis of Puppet Ruby code
 
Point Person(s): Kylo Ginsberg, Andy Parker

| Tasks / Milestones | Milestone |
|--------------------|----------|
| Familiarize with rubocop documentation and warnings it finds in puppet code. | brief writeup of rubocop analysis. 
| Make lib/puppet/pops rubocop clean | PRs merged to puppet-4 branch making `rubocop lib/puppet/pops’ clean. This will likely be a combination of rubocop configuration and code changes. 
| Extend to rest of puppet code base. | PRs merged to puppet-4 branch make `rubocop lib` clean. Same caveats as above. Ideally the same configuration works throughout. 
| CI support for static analysis | add travis and jenkins support for rubocop. 

#### Key Resources (people, departments, links, etc.)
N.A

### Key Objective #3 (from above)
Refactoring of Puppet Modules

Point Person(s): Kylo Ginsberg

| Tasks / Milestones | Due Date |
|--------------------|----------|
| Extract nagios into a separate repo, including tests. | PRs to puppet-4 and new repo to separate nagios. 
| Package puppet to include nagios. | PRs to include nagios in puppet at package time. This will include work with Release Engineering. 
| Stretch goal: do the same for puppet module tool. | PRs to extract and re-package PMT as well. 

### Key Resources (people, departments, links, etc.)
N.A

### Key Objective #4 (from above)
Native Facter support for Solaris
 
Point Person(s): Kylo Ginsberg, Peter Huene

| Tasks / Milestones | Due Date |
|--------------------|----------|
| Build existing native facter on Solaris | PRs merged to support building on Solaris. 
| Identify missing/incorrect facts on Solaris, comparing with ruby facter. | Jira tickets describing work remaining on Solaris. 
| Fill in missing facts on Solaris. Step (b) above will tell us how much work this is. | PRs merged to support facts on Solaris. 

#### Key Resources (people, departments, links, etc.)

Native Facter implementation: https://github.com/puppetlabs/cfacter
Ruby Facter implementation (for reference): https://github.com/puppetlabs/facter

Note that this work is also dependent on some not-yet-complete work by Release Engineering to port the PL toolchain to Solaris. We’ll need to schedule this once that work is complete.

### Key Objective #5 (from above)
Work with community contributions.
 
Point Person(s): Kylo Ginsberg

| Tasks / Milestones | Due Date |
|--------------------|----------|
| Learn about PR triage process | Review open pulls. Attend a PR triage session. 
| Merge a straightforward (no changed needed) community PR. | pair with someone on the team to merge a community PR. Ensure it makes it through CI/FR. Be sure to thank the contributor! 
| Merge a community PR with edits needed. | pair with someone on the team for a PR which requires some back-forth with the contributor. Ensure final PR makes it through CI/FR. Be sure to thank the contributor! 

#### Key Resources (people, departments, links, etc.)

### Key Objective #6 (from above)
Release software

Point Person(s): Kylo Ginsberg

| Tasks / Milestones | Due Date |
|--------------------|----------|
| Z release process, e.g. puppet 3.6.2 | participate in smoke testing for a Z release. Pair on the ticket/commit reconciliation steps. 
| Y release process, e.g. puppet 3.7.0 | participate in ticket/commit reconciliation for a Y release. This is mostly the same as a Z release, but there can be a lot more ticket/commit reconciliation. 

#### Key Resources (people, departments, links, etc.)
N.A
