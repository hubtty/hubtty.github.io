---
layout: splash
permalink: /
hidden: true
header:
  overlay_color: "#1a1d24"
  #overlay_image: /assets/images/banner.jpg
  actions:
    - label: "<i class='fas fa-download'></i> Install now"
      url: "https://github.com/hubtty/hubtty#installation"
excerpt: >
  A console-based interface for Github code reviews.
feature_row:
  - image_path: /assets/images/self-growth.png
    alt: "workflow"
    title: "Review at scale"
    excerpt: "The interface is designed to support a workflow similar to reading network news or mail and to deal with a large number of PRs."
    url: "#review-at-scale"
    btn_class: "btn--primary"
    btn_label: "Learn more"
  - image_path: /assets/images/speedometer.png
    alt: "review faster"
    title: "Review faster"
    excerpt: "Because Hubtty works on files locally, all actions are instantaneous and more enjoyable to work with."
    url: "#review-faster"
    btn_class: "btn--primary"
    btn_label: "Learn more"
  #- image_path: /assets/images/03-PR-view.png
  #  alt: "fully responsive"
  #  title: "Responsive layout"
  #  excerpt: "Hubtty adapts to your console's dimensions. It works equally well on a 80x24 console, or using all of your full HD monitor's real estate."
  #  url: "/docs/layouts/"
  #  btn_class: "btn--primary"
  #  btn_label: "Learn more"
  - image_path: /assets/images/ui.png
    alt: "Highly customizable"
    title: "Highly customizable"
    excerpt: "Colors, keybindings, shortcuts... Customize almost every aspects of Hubtty to match your preferences."
    url: "#highly-customizable"
    btn_class: "btn--primary"
    btn_label: "Learn more"      
---

{% include feature_row %}


# Review at scale

[![Repositories list](/assets/images/01-Repositories-list-small.png)](/assets/images/01-Repositories-list.png){: .align-right}

The interface is designed to support a workflow similar to reading network news
or mail. In particular, it is designed to deal with a large number of Pull
Requests across a large number of repositories.

It is also designed to focus on things that matter during code review:
- branch on which the PR is submitted
- last update
- CI test results
- existing reviews
- quick access to saved search queries

[![PRs list](/assets/images/02-PRs-list-small.png)](/assets/images/02-PRs-list.png){: .align-right}

And reduce noise:
- easily hide pull requests you're not interested in
- reviewed PRs are hidden and re-appear once they are updated
- filter robot comments

# Review while on the go

[![PRs list](/assets/images/03-PR-view-small.png)](/assets/images/03-PR-view.png){: .align-right}

Hubtty works seamlessly offline or online. Hubtty syncs information about pull
requests in subscribed repositories to a local database and local git repos.
All of the actions that it performs are first recorded in that database, and
are then transmitted to Github. If Hubtty is unable to contact Github for any
reason, it will continue to operate against the local database, and once it
re-establishes contact, it will process any pending changes.

If you review a pull request while offline with a positive vote, and someone
else leaves a negative vote on that pull request before Hubtty is able to
upload your review, Hubtty will detect the situation and mark the pull request
as "held" so that you may re-inspect the pull request and any new comments
before uploading the review.

# Review faster

User actions modify locally cached content and need not wait for server
interaction, making the whole experience of navigating Pull Requests much more
enjoyable.

[![PRs list](/assets/images/03-PR-view-small.png)](/assets/images/03-PR-view.png){: .align-left}

Because Hubtty downloads all pull requests to local git repos, a single command
instructs it to checkout a pull request into that repo for detailed examination
or testing of larger pull requests.

Hubtty also offers quality of life improvements such as
[dashboards](https://hubtty.readthedocs.io/en/latest/configuration.html#dashboards)
for saved search queries,
[hotkeys](https://hubtty.readthedocs.io/en/latest/configuration.html#reviewkeys)
to perform immediate reviews, or the ability to mass edit PRs.

TODO Add a screenshot of a search dashboard


# Highly customizable

Hubtty includes [many
options](https://hubtty.readthedocs.io/en/latest/configuration.html#configuration-reference)
to integrate better with your environment and preferences:
- Re-bind every action with custom
[keybindings](https://hubtty.readthedocs.io/en/latest/configuration.html#keymaps)
to take advantage of your muscle-memory.
- Change the look and feel with a custom
[palette](https://hubtty.readthedocs.io/en/latest/configuration.html#palettes) for eye-candy themes.
- Create links pointing to your issue tracker when pull requests reference issues, using [custom matchers](https://hubtty.readthedocs.io/en/latest/configuration.html#commentlinks).
- Define [review keys](https://hubtty.readthedocs.io/en/latest/configuration.html#reviewkeys) to leave pre-defined comments with a single key stroke.
- And many more...
