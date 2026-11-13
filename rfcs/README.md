# Changing the spec: the RFC process

An RFC (request for comments) is a public proposal to change the rating spec. Every change to the official spec starts as one, so anyone can see what changed, why, and what evidence supported it.

## Steps

1. **Raise the idea.** Open an issue with the [rating spec change form](https://github.com/openpickleball/.github/issues/new/choose). Discussion there shows whether the idea is worth a full proposal.
2. **Write the RFC.** Copy [0000-template.md](0000-template.md) to `rfcs/0000-short-title.md` and fill it in. Open a pull request in this repository. When the pull request is open, rename the file to use the pull request number, such as `rfcs/0012-short-title.md`.
3. **Public comment.** Anyone can comment on the pull request. The author updates the RFC in response. Evidence matters most: how the change affects predictive accuracy and calibration on matches the engine has not seen.
4. **Decision.** The governing board approves or declines the RFC by a public vote, as [GOVERNANCE.md](https://github.com/openpickleball/.github/blob/main/GOVERNANCE.md) describes, and the result and reasons are recorded on the pull request. Until the board is seated, no RFC can be approved and no official spec version can be published.
5. **Publish.** An approved RFC is merged. The spec change follows in its own pull request, which adds a new versioned file under `spec/`, an entry in `CHANGELOG.md`, and the engine config version that implements it.

A declined RFC is merged too, marked as declined, so the record stays complete.

## What does not need an RFC

Typo fixes and wording clarifications with no effect on any rating are patch changes. They need a pull request and review, but not an RFC.
