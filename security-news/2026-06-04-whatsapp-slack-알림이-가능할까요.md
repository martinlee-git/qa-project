# Whatsapp Slack 알림이 가능할까요?
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/whatsapp-slack-notifications-could.html
- Published At: unknown
- Collected At: 2026-06-04T00:39:54.382Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Whatsapp-Slack-374fc93aec578195a5d9d5677c78eb72
- Original Title: Whatsapp Slack Notifications Could
## Summary
중독된 Android 알림은 악성 앱 없이 Google Gemini의 음성 어시스턴트를 탈취할 수 있습니다. WhatsApp, Slack, SMS, Signal, Instagram 또는 메신저에서 보내는 단일 알림으로 인해 Android에서 Google Gemini의 음성 어시스턴트가 하이재킹되어 피해자의 연결된 창을 열거나, 상사의 메시지를 위조하거나, 전화기를 Zoom 통화에 연결하거나, 조용히 장기 기억을 독살시킬 수 있습니다. 휴대폰에 악성 앱이 필요하지 않습니다. 보조자는 적대적인 알림을 유용한 컨텍스트로 처리하면 되었습니다. SafeBreach의 Or Yair가 발표한 연구는 팀의 초기 "Invitation Is All You Need" 작업을 따릅니다. 이 작업은 악성 Google Calend를 통해 유사한 트릭을 수행했습니다.

## Original Description

Poisoned Android notifications could hijack Google Gemini’s voice assistant without a malicious app.
## Key Points
- 중독된 Android 알림은 악성 앱 없이 Google Gemini의 음성 어시스턴트를 탈취할 수 있습니다.
- WhatsApp, Slack, SMS, Signal, Instagram 또는 메신저에서 보내는 단일 알림으로 인해 Android에서 Google Gemini의 음성 어시스턴트가 하이재킹되어 피해자의 연결된 창을 열거나, 상사의 메시지를 위조하거나, 전화기를 Zoom 통화에 연결하거나, 조용히 장기 기억을 독살시킬 수 있습니다.
- 휴대폰에 악성 앱이 필요하지 않습니다.
## Excerpt
WhatsApp, Slack, SMS, Signal, Instagram 또는 메신저에서 보내는 단일 알림으로 인해 Android에서 Google Gemini의 음성 어시스턴트가 하이재킹되어 피해자의 연결된 창을 열거나, 상사의 메시지를 위조하거나, 전화기를 Zoom 통화에 연결하거나, 조용히 장기 기억을 독살시킬 수 있습니다. 휴대폰에 악성 앱이 필요하지 않습니다. 보조자는 적대적인 알림을 유용한 컨텍스트로 처리하면 되었습니다. SafeBreach의 Or Yair가 발표한 연구는 악의적인 Google 캘린더 초대를 통해 유사한 트릭을 수행한 팀의 초기 "Invitation Is All You Need" 작업을 따릅니다. 그 후 Google은 간접적인 프롬프트 주입에 대해 Gemini를 강화했습니다. Yair는 새로운 방어를 우회하는 방법을 찾았습니다. Google은 이후 이를 패치했으며 SafeBreach는 이 문제에 대한 CVE를 나열하지 않았으며 해당 기술이 실제로 사용되었다는 증거도 없습니다. Android에서 Gemini의 유틸리티 기능은 WhatsApp과 같은 앱의 알림을 포함하여 알림을 읽고 응답할 수 있습니다. 이 벡터는 Android 전용으로 유지되는 iOS 또는 웹에서는 사용할 수 없습니다. Yair는 이러한 알림을 읽는 에이전트가 해당 텍스트를 조치를 취할 수 있는 지침으로 취급한다는 사실을 발견했습니다. 따라서 휴대폰에 알림을 보낼 수 있는 모든 것은 "실질적으로 무한"이라고 불리는 공격 표면 Yair인 페이로드를 전달할 수 있습니다.