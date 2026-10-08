# Offline knowledge prototype: proposed delivery

This is a proposed implementation approach. The complete offline stack has not
yet been built or tested as part of this portfolio.

## Components and responsibilities

| Component | Role | Questions to resolve |
|---|---|---|
| Ubuntu or Pop!_OS | Mini-PC host | Hardware, storage, installation access and recovery method |
| Docker Compose | Service configuration and lifecycle | Tested versions, persistent data and startup dependencies |
| Ollama and a local web interface | Local AI | Model fit, response expectations, user count and access |
| Kiwix | Offline reference library | Required archives, language, storage and refresh process |
| Calibre-Web | Book library | Content, formats, permissions and catalog organization |
| Kolibri | Educational content | Channels, languages, storage and packaging |
| Local portal / reverse proxy | Service entry point | Local addressing, navigation and access requirements |
| Optional maps | Offline map viewing | Region, detail, dataset size and separate scope |

Final versions and content licenses would be checked when selecting components.
Applicable third-party notices accompany the delivered stack.

## Acceptance checks to agree before implementation

1. **Install:** scripts and documented prerequisites produce the agreed services
   on the target or agreed equivalent test hardware.
2. **Operate offline:** after provisioning, agreed AI and content tasks work with
   external connectivity disabled. Test notes distinguish blocked outbound requests
   from features that require the internet.
3. **Restart:** a reboot restores agreed services and preserves content/settings.
   The operator can recognize and recover a failed service.
4. **Update and recover:** exercise a representative update and rollback in the
   agreed test environment. Document backup contents, restore steps and the offline
   content import process.
5. **Hand over:** deliver configuration, setup/update scripts, folder conventions,
   test results and an operator walkthrough.

Response-time targets, supported user count and recovery expectations are agreed
before they become acceptance commitments.

## Information needed to quote

- CPU, RAM, storage, graphics and current operating system.
- Required languages, content collections, volume and optional map region.
- User count and access from the machine itself or a local network.
- Whether offline requirements include installation and updates from removable media.
- Deadline, access arrangements, existing work and the customer review process.

## Deliverables and ownership

The engagement can include a customer repository with container configuration,
project-specific scripts, documentation and acceptance records. Access, ownership
and support terms are agreed before implementation. Existing business systems and
unrelated source remain outside the project. The private portfolio implementation
does not prevent delivery of the agreed customer work.
