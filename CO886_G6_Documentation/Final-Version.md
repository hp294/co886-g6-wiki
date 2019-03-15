Our final version of the HEAT program incorporates a number of modifications which improve the UI for visually impaired users. 

At the outset of the project the team liaised with users and developed a series of user stories which guided the development process, in particular the user noted that the software would be deployed in an environment where it would be used primarily by visually impaired users, and as such the default UI should be accessible, with no particular requirement for a standard version. This requirement guided our decision to implement our modifications as permanent changes rather than optional features.

Our research highlighted a number of potential features which were assigned priorities based on the potential impact of the feature and the feasibility of implementation within the project timeframe. The result of this process was the set of requirements listed above, all of which have been successfully incorporated into the final version. Following user testing, some additional changes were made to the UI, highlighting the importance of user involvement in the development process.

Given more time, the team identified a number of additional features which could have implemented including a text to voice feature and voice only control, however it was agreed early in the project to focus on good quality implementation of the high priority requirements.

There were some notable difficulties encountered during the project. One particular issue arose when the merging of a feature branch overwrote changes which had already been made to the master branch. To resolve this issue we used the revert commit feature on GitLab, followed by a pull and rebase in Eclipse, resolving the conflicts before re-merging the feature branch.

The ability to control versions and revert on GitLab made the collaboration process much smoother and allowed for team members to work simultaneously on different features. The Eclipse IDE was also vital for the completion of the project. The Git staging feature was utilised heavily throughout the project, and other features such as, debugging, method suggestion, and the ability to run the program from the IDE proved to be very useful in modifying a reasonably large piece of software in a relatively short time.

**Report**:[Group_6_-_report-v9.doc](uploads/75d6c1245f2eea093240da9b1e29a5f2/Group_6_-_report-v9.doc)