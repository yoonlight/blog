# Git

## Commit

1. A commit message is comprised of a subject ( i.e summary), body, and footer, with both the body and footer being optional.
- 커밋 메시지는 subject(summary), body, footer로 구성되어 있다
- body와 footer는 optional 하다
2. Limit the subject line to 50 characters.
- subject는 50글자 이하로 제한한다.
    1. The subject is a single line that best sums up the changes made in the commit.
        1. subject는 한줄로 작성한다
        2. subject의 내용은 커밋에서 변경점을 전부 합친것이다.
    3. The act of summarising your commit is a good practice inherently in any version control system.
        1. 당신의 커밋을 요약하는 것은 어느 버전 컨트롤 시스템에서도 좋은 관행이다
    5. It helps others (or a later you) find relevant commits more quickly.
        1. 커밋을 빠르게 찾는데 도움이 된다.
3. Capitalise the first letter of the subject line.
- Subject의 첫글자는 대문자 사용해라
4. Don’t put a period ( . ) at the end of the subject line.
- subject에 "."를 사용하지 마라
5. Put a blank line between the subject line and the body & also between body and footer.
- subject, body, footer 사이에 빈줄을 삽입해라
6. Wrap the commit body at 72 characters.
- 커밋 body를 72글자로 감싸라 (한줄에 72글자 까지 작성후 넘어갈 경우 띄어라)
    - The body text is used to provide more details regarding the changes made in the commit.
    - body 텍스트는 커밋에 만들어진 변화의 관한 상세한 정보를 제공하기 위해서 사용된다
7. Write the commit body in bullets (OPTIONAL).
- commit body를 글머리 기호에 작성해라
    - Commit body looks clean when written in terms of bullets.
8. Use imperative mood
- 명령어를 사용해라
    - Example: Say Add instead of Added
    - Say Fix instead of Fixed, Fixes → Use present tense imperative for the subject line and present tense for body text
    - subject에 현재 시제 명령형을 body에 현재 시제를 사용해라
    - The present imperative should be used for the subject line of commit messages.
        - 명령어는 subject line에 사용되어야 한다
    - This is what has been standardized by git itself.
9. Describe what and why, but not how.
- 어떻게가 아닌 무엇을, 왜를 기술해라
    - Maybe Mention Which component is changed.
        - 어느 컴포넌트가 변경되었는지를 언급해라
    - Just keep your mind on the purpose, not the implementation.
    - 구현이 아닌 당신의 목적을 기술해라
    - Most of the modern bug-tracking and project management systems provide integration with the source control repository, 
    - but even if they don’t, you can still drop task/ticket numbers in the commit message – something like this. 
    - Of course – don’t rely on this being the only description of your message.
10. Footer contains issue no. and ticket if needed (OPTIONAL).
- Footer에는 필요시 issue no., ticket을 포함한다
    - The footer text is found immediately below the body and is a place to reference issues related to the commit changes. 
        - Footer 텍스트는 body아래에 있으며 커밋 변경에 관련된 issue 참고에 사용된다
    - Example Mention Issue no. in GitHub and If you are using JIRA to manage your project
       - Issue no. 는 Github에서, 


### Reference

* <https://medium.com/@hritik.jaiswal/how-to-write-a-good-commit-message-9d2d533b9052>
* <https://www.conventionalcommits.org/en/v1.0.0/>
