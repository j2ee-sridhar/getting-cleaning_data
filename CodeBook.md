



<!DOCTYPE html>
<html lang="en" class="">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    
    
    <title>Coursera-Data-Science-Getting-and-Cleaning-Data/CodeBook.md at master Â· yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-144.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data" name="twitter:title" /><meta content="Coursera-Data-Science-Getting-and-Cleaning-Data - This repository is mainly for the way we preprocessing the data" name="twitter:description" /><meta content="https://avatars0.githubusercontent.com/u/8656557?v=2&amp;s=400" name="twitter:image:src" />
<meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="https://avatars0.githubusercontent.com/u/8656557?v=2&amp;s=400" property="og:image" /><meta content="yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data" property="og:title" /><meta content="https://github.com/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data" property="og:url" /><meta content="Coursera-Data-Science-Getting-and-Cleaning-Data - This repository is mainly for the way we preprocessing the data" property="og:description" />

      <meta name="browser-stats-url" content="/_stats">
    <link rel="assets" href="https://assets-cdn.github.com/">
    <link rel="conduit-xhr" href="https://ghconduit.com:25035">
    <link rel="xhr-socket" href="/_sockets">
    <meta name="pjax-timeout" content="1000">

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>
      <meta name="google-analytics" content="UA-3769691-2">

    <meta content="collector.githubapp.com" name="octolytics-host" /><meta content="collector-cdn.github.com" name="octolytics-script-host" /><meta content="github" name="octolytics-app-id" /><meta content="0E63607A:26CE:195CAC1:544A8FCF" name="octolytics-dimension-request_id" /><meta content="3930639" name="octolytics-actor-id" /><meta content="j2ee-sridhar" name="octolytics-actor-login" /><meta content="5e680832109d5f6bfdfe754479b7b5640a4b53431a39e1c5fd3a6724c917a09a" name="octolytics-actor-hash" />
    
    <meta content="Rails, view, blob#show" name="analytics-event" />

    
    
    <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">


    <meta content="authenticity_token" name="csrf-param" />
<meta content="6xS3jHUqBwhQk7yDVYLfKDvTO4XedgFPtwdzGM+3g1G0/1DEHT+XeoJOynaI+hLg4iB0GnNkYyD4ZZgd/ugPNg==" name="csrf-token" />

    <link href="https://assets-cdn.github.com/assets/github-d41b723d1561b1cbd027687846dcf560227d28ed108555db87df65e4647433ad.css" media="all" rel="stylesheet" type="text/css" />
    <link href="https://assets-cdn.github.com/assets/github2-e601e4dc2eec6decc441b9f7e15eec77891539a1a5e2d8af7af600d1d061a150.css" media="all" rel="stylesheet" type="text/css" />
    
    


    <meta http-equiv="x-pjax-version" content="f33e34fc7e40286ba76217947ed67f44">

      
  <meta name="description" content="Coursera-Data-Science-Getting-and-Cleaning-Data - This repository is mainly for the way we preprocessing the data">
  <meta name="go-import" content="github.com/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data git https://github.com/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data.git">

  <meta content="8656557" name="octolytics-dimension-user_id" /><meta content="yelangya" name="octolytics-dimension-user_login" /><meta content="23670974" name="octolytics-dimension-repository_id" /><meta content="yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="23670974" name="octolytics-dimension-repository_network_root_id" /><meta content="yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/commits/master.atom" rel="alternate" title="Recent Commits to Coursera-Data-Science-Getting-and-Cleaning-Data:master" type="application/atom+xml">

  </head>


  <body class="logged_in  env-production windows vis-public page-blob">
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>
    <div class="wrapper">
      
      
      
      


      <div class="header header-logged-in true" role="banner">
  <div class="container clearfix">

    <a class="header-logo-invertocat" href="https://github.com/" data-hotkey="g d" aria-label="Homepage" ga-data-click="Header, go to dashboard, icon:logo">
  <span class="mega-octicon octicon-mark-github"></span>
</a>


      <div class="site-search repo-scope js-site-search" role="search">
          <form accept-charset="UTF-8" action="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/search" class="js-site-search-form" data-global-search-url="/search" data-repo-search-url="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
  <input type="text"
    class="js-site-search-field is-clearable"
    data-hotkey="s"
    name="q"
    placeholder="Search"
    data-global-scope-placeholder="Search GitHub"
    data-repo-scope-placeholder="Search"
    tabindex="1"
    autocapitalize="off">
  <div class="scope-badge">This repository</div>
</form>
      </div>
      <ul class="header-nav left" role="navigation">
        <li class="header-nav-item explore">
          <a class="header-nav-link" href="/explore" data-ga-click="Header, go to explore, text:explore">Explore</a>
        </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="https://gist.github.com" data-ga-click="Header, go to gist, text:gist">Gist</a>
          </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="/blog" data-ga-click="Header, go to blog, text:blog">Blog</a>
          </li>
        <li class="header-nav-item">
          <a class="header-nav-link" href="https://help.github.com" data-ga-click="Header, go to help, text:help">Help</a>
        </li>
      </ul>

    
<ul class="header-nav user-nav right" id="user-links">
  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link name" href="/j2ee-sridhar" data-ga-click="Header, go to profile, text:username">
      <img alt="j2ee-sridhar" class="avatar" data-user="3930639" height="20" src="https://avatars3.githubusercontent.com/u/3930639?v=2&amp;s=40" width="20" />
      <span class="css-truncate">
        <span class="css-truncate-target">j2ee-sridhar</span>
      </span>
    </a>
  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link js-menu-target tooltipped tooltipped-s" href="#" aria-label="Create new..." data-ga-click="Header, create new, icon:add">
      <span class="octicon octicon-plus"></span>
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      
<ul class="dropdown-menu">
  <li>
    <a href="/new"><span class="octicon octicon-repo"></span> New repository</a>
  </li>
  <li>
    <a href="/organizations/new"><span class="octicon octicon-organization"></span> New organization</a>
  </li>


    <li class="dropdown-divider"></li>
    <li class="dropdown-header">
      <span title="yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data">This repository</span>
    </li>
      <li>
        <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/issues/new"><span class="octicon octicon-issue-opened"></span> New issue</a>
      </li>
</ul>

    </div>
  </li>

  <li class="header-nav-item">
        <a href="/notifications" aria-label="You have no unread notifications" class="header-nav-link notification-indicator tooltipped tooltipped-s" data-ga-click="Header, go to notifications, icon:read" data-hotkey="g n">
        <span class="mail-status all-read"></span>
        <span class="octicon octicon-inbox"></span>
</a>
  </li>

  <li class="header-nav-item">
    <a class="header-nav-link tooltipped tooltipped-s" href="/settings/profile" id="account_settings" aria-label="Settings" data-ga-click="Header, go to settings, icon:settings">
      <span class="octicon octicon-gear"></span>
    </a>
  </li>

  <li class="header-nav-item">
    <form accept-charset="UTF-8" action="/logout" class="logout-form" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="5eom8C9sTK6dl2jonk2s2LKnTZN2svT0FGNcXSExAexLvHCUUn5pewYmHk+Irbdzy7+OFZkXLmQJojRS15vY4g==" /></div>
      <button class="header-nav-link sign-out-button tooltipped tooltipped-s" aria-label="Sign out" data-ga-click="Header, sign out, icon:logout">
        <span class="octicon octicon-sign-out"></span>
      </button>
</form>  </li>

</ul>


    
  </div>
</div>

      

        


      <div id="start-of-content" class="accessibility-aid"></div>
          <div class="site" itemscope itemtype="http://schema.org/WebPage">
    <div id="js-flash-container">
      
    </div>
    <div class="pagehead repohead instapaper_ignore readability-menu">
      <div class="container">
        
<ul class="pagehead-actions">

    <li class="subscription">
      <form accept-charset="UTF-8" action="/notifications/subscribe" class="js-social-container" data-autosubmit="true" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="TH9UyUcYRrQWh68WO6EHRkdSRoNdASS6YrUUUvZf3wtmNkMAJnHLaQCG8W5Fw/uoSskFyyEhi/XbYPGhmDK2sQ==" /></div>  <input id="repository_id" name="repository_id" type="hidden" value="23670974" />

    <div class="select-menu js-menu-container js-select-menu">
      <a class="social-count js-social-count" href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/watchers">
        1
      </a>
      <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/subscription"
        class="minibutton select-menu-button with-count js-menu-target" role="button" tabindex="0" aria-haspopup="true">
        <span class="js-select-button">
          <span class="octicon octicon-eye"></span>
          Watch
        </span>
      </a>

      <div class="select-menu-modal-holder">
        <div class="select-menu-modal subscription-menu-modal js-menu-content" aria-hidden="true">
          <div class="select-menu-header">
            <span class="select-menu-title">Notifications</span>
            <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
          </div> <!-- /.select-menu-header -->

          <div class="select-menu-list js-navigation-container" role="menu">

            <div class="select-menu-item js-navigation-item selected" role="menuitem" tabindex="0">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <div class="select-menu-item-text">
                <input checked="checked" id="do_included" name="do" type="radio" value="included" />
                <h4>Not watching</h4>
                <span class="description">Be notified when participating or @mentioned.</span>
                <span class="js-select-button-text hidden-select-button-text">
                  <span class="octicon octicon-eye"></span>
                  Watch
                </span>
              </div>
            </div> <!-- /.select-menu-item -->

            <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
              <span class="select-menu-item-icon octicon octicon octicon-check"></span>
              <div class="select-menu-item-text">
                <input id="do_subscribed" name="do" type="radio" value="subscribed" />
                <h4>Watching</h4>
                <span class="description">Be notified of all conversations.</span>
                <span class="js-select-button-text hidden-select-button-text">
                  <span class="octicon octicon-eye"></span>
                  Unwatch
                </span>
              </div>
            </div> <!-- /.select-menu-item -->

            <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <div class="select-menu-item-text">
                <input id="do_ignore" name="do" type="radio" value="ignore" />
                <h4>Ignoring</h4>
                <span class="description">Never be notified.</span>
                <span class="js-select-button-text hidden-select-button-text">
                  <span class="octicon octicon-mute"></span>
                  Stop ignoring
                </span>
              </div>
            </div> <!-- /.select-menu-item -->

          </div> <!-- /.select-menu-list -->

        </div> <!-- /.select-menu-modal -->
      </div> <!-- /.select-menu-modal-holder -->
    </div> <!-- /.select-menu -->

</form>
    </li>

  <li>
    
  <div class="js-toggler-container js-social-container starring-container ">

    <form accept-charset="UTF-8" action="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/unstar" class="js-toggler-form starred js-unstar-button" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="/idnYAw7qHBGZ2GimXYPjnVrjBx7woKOyxb9IbMU8c6EAZwjfZkscowsIiWm/VBNHHrquE1MfMrtuZvQTCWuEg==" /></div>
      <button
        class="minibutton with-count js-toggler-target star-button"
        aria-label="Unstar this repository" title="Unstar yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data">
        <span class="octicon octicon-star"></span>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/stargazers">
          0
        </a>
</form>
    <form accept-charset="UTF-8" action="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/star" class="js-toggler-form unstarred js-star-button" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="y8KyRA/CP2xw5JYrdiNSq5qICxePwgIbSjAFyvS3lQ0DJm1Zq2vBZR7jhkXNUmz1ahgS/KxPnQcHtWxGPR6Ynw==" /></div>
      <button
        class="minibutton with-count js-toggler-target star-button"
        aria-label="Star this repository" title="Star yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data">
        <span class="octicon octicon-star"></span>
        Star
      </button>
        <a class="social-count js-social-count" href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/stargazers">
          0
        </a>
</form>  </div>

  </li>


        <li>
          <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/fork" class="minibutton with-count js-toggler-target fork-button tooltipped-n" title="Fork your own copy of yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data to your account" aria-label="Fork your own copy of yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data to your account" rel="nofollow" data-method="post">
            <span class="octicon octicon-repo-forked"></span>
            Fork
          </a>
          <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/network" class="social-count">0</a>
        </li>

</ul>

        <h1 itemscope itemtype="http://data-vocabulary.org/Breadcrumb" class="entry-title public">
          <span class="mega-octicon octicon-repo"></span>
          <span class="author"><a href="/yelangya" class="url fn" itemprop="url" rel="author"><span itemprop="title">yelangya</span></a></span><!--
       --><span class="path-divider">/</span><!--
       --><strong><a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data" class="js-current-repository js-repo-home-link" data-pjax-container-selector="#js-repo-pjax-container">Coursera-Data-Science-Getting-and-Cleaning-Data</a></strong>

          <span class="page-context-loader">
            <img alt="" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
          </span>

        </h1>
      </div><!-- /.container -->
    </div><!-- /.repohead -->

    <div class="container">
      <div class="repository-with-sidebar repo-container new-discussion-timeline  ">
        <div class="repository-sidebar clearfix">
            
<div class="sunken-menu vertical-right repo-nav js-repo-nav js-sidenav-container-pjax js-octicon-loaders" role="navigation" data-issue-count-url="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/issues/counts" data-pjax-container-selector="#js-repo-pjax-container">
  <div class="sunken-menu-contents">
    <ul class="sunken-menu-group">
      <li class="tooltipped tooltipped-w" aria-label="Code">
        <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data" aria-label="Code" class="selected js-selected-navigation-item sunken-menu-item" data-hotkey="g c" data-pjax="true" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data">
          <span class="octicon octicon-code"></span> <span class="full-word">Code</span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>

        <li class="tooltipped tooltipped-w" aria-label="Issues">
          <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/issues" aria-label="Issues" class="js-selected-navigation-item sunken-menu-item js-disable-pjax" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/issues">
            <span class="octicon octicon-issue-opened"></span> <span class="full-word">Issues</span>
            <span class="js-issue-replace-counter"></span>
            <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>        </li>

      <li class="tooltipped tooltipped-w" aria-label="Pull Requests">
        <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/pulls" aria-label="Pull Requests" class="js-selected-navigation-item sunken-menu-item js-disable-pjax" data-hotkey="g p" data-selected-links="repo_pulls /yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/pulls">
            <span class="octicon octicon-git-pull-request"></span> <span class="full-word">Pull Requests</span>
            <span class="js-pull-replace-counter"></span>
            <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>


        <li class="tooltipped tooltipped-w" aria-label="Wiki">
          <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/wiki" aria-label="Wiki" class="js-selected-navigation-item sunken-menu-item js-disable-pjax" data-hotkey="g w" data-selected-links="repo_wiki /yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/wiki">
            <span class="octicon octicon-book"></span> <span class="full-word">Wiki</span>
            <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>        </li>
    </ul>
    <div class="sunken-menu-separator"></div>
    <ul class="sunken-menu-group">

      <li class="tooltipped tooltipped-w" aria-label="Pulse">
        <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/pulse/weekly" aria-label="Pulse" class="js-selected-navigation-item sunken-menu-item" data-pjax="true" data-selected-links="pulse /yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/pulse/weekly">
          <span class="octicon octicon-pulse"></span> <span class="full-word">Pulse</span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>

      <li class="tooltipped tooltipped-w" aria-label="Graphs">
        <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/graphs" aria-label="Graphs" class="js-selected-navigation-item sunken-menu-item" data-pjax="true" data-selected-links="repo_graphs repo_contributors /yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/graphs">
          <span class="octicon octicon-graph"></span> <span class="full-word">Graphs</span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>
    </ul>


  </div>
</div>

              <div class="only-with-full-nav">
                
  
<div class="clone-url open"
  data-protocol-type="http"
  data-url="/users/set_protocol?protocol_selector=http&amp;protocol_type=clone">
  <h3><span class="text-emphasized">HTTPS</span> clone URL</h3>
  <div class="input-group">
    <input type="text" class="input-mini input-monospace js-url-field"
           value="https://github.com/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data.git" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-clipboard-text="https://github.com/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data.git" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="clone-url "
  data-protocol-type="ssh"
  data-url="/users/set_protocol?protocol_selector=ssh&amp;protocol_type=clone">
  <h3><span class="text-emphasized">SSH</span> clone URL</h3>
  <div class="input-group">
    <input type="text" class="input-mini input-monospace js-url-field"
           value="git@github.com:yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data.git" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-clipboard-text="git@github.com:yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data.git" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="clone-url "
  data-protocol-type="subversion"
  data-url="/users/set_protocol?protocol_selector=subversion&amp;protocol_type=clone">
  <h3><span class="text-emphasized">Subversion</span> checkout URL</h3>
  <div class="input-group">
    <input type="text" class="input-mini input-monospace js-url-field"
           value="https://github.com/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-clipboard-text="https://github.com/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>


<p class="clone-options">You can clone with
      <a href="#" class="js-clone-selector" data-protocol="http">HTTPS</a>,
      <a href="#" class="js-clone-selector" data-protocol="ssh">SSH</a>,
      or <a href="#" class="js-clone-selector" data-protocol="subversion">Subversion</a>.
  <a href="https://help.github.com/articles/which-remote-url-should-i-use" class="help tooltipped tooltipped-n" aria-label="Get help on which URL is right for you.">
    <span class="octicon octicon-question"></span>
  </a>
</p>


  <a href="github-windows://openRepo/https://github.com/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data" class="minibutton sidebar-button" title="Save yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data to your computer and use it in GitHub Desktop." aria-label="Save yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data to your computer and use it in GitHub Desktop.">
    <span class="octicon octicon-device-desktop"></span>
    Clone in Desktop
  </a>

                <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/archive/master.zip"
                   class="minibutton sidebar-button"
                   aria-label="Download the contents of yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data as a zip file"
                   title="Download the contents of yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data as a zip file"
                   rel="nofollow">
                  <span class="octicon octicon-cloud-download"></span>
                  Download ZIP
                </a>
              </div>
        </div><!-- /.repository-sidebar -->

        <div id="js-repo-pjax-container" class="repository-content context-loader-container" data-pjax-container>
          

<a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/blob/d052fb89249be83d311a67c1203cd13ad296280c/CodeBook.md" class="hidden js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:1aca0fc8831234faaf248aa763c5b091 -->

<div class="file-navigation">
  
<div class="select-menu js-menu-container js-select-menu left">
  <span class="minibutton select-menu-button js-menu-target css-truncate" data-hotkey="w"
    data-master-branch="master"
    data-ref="master"
    title="master"
    role="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <span class="octicon octicon-git-branch"></span>
    <i>branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </span>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <span class="select-menu-title">Switch branches/tags</span>
        <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
      </div> <!-- /.select-menu-header -->

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" class="js-select-menu-tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" class="js-select-menu-tab">Tags</a>
            </li>
          </ul>
        </div><!-- /.select-menu-tabs -->
      </div><!-- /.select-menu-filters -->

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <div class="select-menu-item js-navigation-item ">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/blob/gh-pages/CodeBook.md"
                 data-name="gh-pages"
                 data-skip-pjax="true"
                 rel="nofollow"
                 class="js-navigation-open select-menu-item-text css-truncate-target"
                 title="gh-pages">gh-pages</a>
            </div> <!-- /.select-menu-item -->
            <div class="select-menu-item js-navigation-item selected">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/blob/master/CodeBook.md"
                 data-name="master"
                 data-skip-pjax="true"
                 rel="nofollow"
                 class="js-navigation-open select-menu-item-text css-truncate-target"
                 title="master">master</a>
            </div> <!-- /.select-menu-item -->
        </div>

          <div class="select-menu-no-results">Nothing to show</div>
      </div> <!-- /.select-menu-list -->

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div> <!-- /.select-menu-list -->

    </div> <!-- /.select-menu-modal -->
  </div> <!-- /.select-menu-modal-holder -->
</div> <!-- /.select-menu -->

  <div class="button-group right">
    <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/find/master"
          class="js-show-file-finder minibutton empty-icon tooltipped tooltipped-s"
          data-pjax
          data-hotkey="t"
          aria-label="Quickly jump between files">
      <span class="octicon octicon-list-unordered"></span>
    </a>
    <button class="js-zeroclipboard minibutton zeroclipboard-button"
          data-clipboard-text="CodeBook.md"
          aria-label="Copy to clipboard"
          data-copied-hint="Copied!">
      <span class="octicon octicon-clippy"></span>
    </button>
  </div>

  <div class="breadcrumb">
    <span class='repo-root js-repo-root'><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data" class="" data-branch="master" data-direction="back" data-pjax="true" itemscope="url"><span itemprop="title">Coursera-Data-Science-Getting-and-Cleaning-Data</span></a></span></span><span class="separator"> / </span><strong class="final-path">CodeBook.md</strong>
  </div>
</div>


  <deferred-content class="commit commit-loader file-history-tease" src="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/contributors/master/CodeBook.md">
    <div class="file-history-tease-header">
      Fetching contributors&hellip;
    </div>

    <div class="participation">
      <p class="loader-loading"><img alt="" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32-EAF2F5.gif" width="16" /></p>
      <p class="loader-error">Cannot retrieve contributors at this time</p>
    </div>
  </deferred-content>

<div class="file-box">
  <div class="file">
    <div class="meta clearfix">
      <div class="info file-name">
          <span>164 lines (137 sloc)</span>
          <span class="meta-divider"></span>
        <span>6.386 kb</span>
      </div>
      <div class="actions">
        <div class="button-group">
          <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/raw/master/CodeBook.md" class="minibutton " id="raw-url">Raw</a>
            <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/blame/master/CodeBook.md" class="minibutton js-update-url-with-hash">Blame</a>
          <a href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/commits/master/CodeBook.md" class="minibutton " rel="nofollow">History</a>
        </div><!-- /.button-group -->

          <a class="octicon-button tooltipped tooltipped-nw"
             href="github-windows://openRepo/https://github.com/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data?branch=master&amp;filepath=CodeBook.md" aria-label="Open this file in GitHub for Windows">
              <span class="octicon octicon-device-desktop"></span>
          </a>

              <a class="octicon-button tooltipped tooltipped-n js-update-url-with-hash"
                 aria-label="Clicking this button will fork this project so you can edit the file"
                 href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/edit/master/CodeBook.md"
                 data-method="post" rel="nofollow"><span class="octicon octicon-pencil"></span></a>

            <a class="octicon-button danger tooltipped tooltipped-s"
               href="/yelangya/Coursera-Data-Science-Getting-and-Cleaning-Data/delete/master/CodeBook.md"
               aria-label="Fork this project and delete file"
               data-method="post" data-test-id="delete-blob-file" rel="nofollow">
          <span class="octicon octicon-trashcan"></span>
        </a>
      </div><!-- /.actions -->
    </div>
      <div id="readme" class="blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="mainContentOfPage"><h1>
<a name="user-content-codebook" class="anchor" href="#codebook" aria-hidden="true"><span class="octicon octicon-link"></span></a>CodeBook</h1>

<p>The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. </p>

<p>Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). </p>

<p>Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). </p>

<p>These signals were used to estimate variables of the feature vector for each pattern:<br>
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.</p>

<p>Features include 79 columns from columns 3 to columns 81, and they are:</p>

<ul class="task-list">
<li>tBodyAcc.mean...X</li>
<li>tBodyAcc.mean...Y</li>
<li>tBodyAcc.mean...Z</li>
<li>tGravityAcc.mean...X</li>
<li>tGravityAcc.mean...Y</li>
<li>tGravityAcc.mean...Z</li>
<li>tBodyAccJerk.mean...X</li>
<li>tBodyAccJerk.mean...Y</li>
<li>tBodyAccJerk.mean...Z</li>
<li>tBodyGyro.mean...X</li>
<li>tBodyGyro.mean...Y</li>
<li>tBodyGyro.mean...Z</li>
<li>tBodyGyroJerk.mean...X</li>
<li>tBodyGyroJerk.mean...Y</li>
<li>tBodyGyroJerk.mean...Z</li>
<li>tBodyAccMag.mean..</li>
<li>tGravityAccMag.mean..</li>
<li>tBodyAccJerkMag.mean..</li>
<li>tBodyGyroMag.mean.. </li>
<li>tBodyGyroJerkMag.mean.. </li>
<li>fBodyAcc.mean...X<br>
</li>
<li>fBodyAcc.mean...Y<br>
</li>
<li>fBodyAcc.mean...Z<br>
</li>
<li>fBodyAcc.meanFreq...X<br>
</li>
<li>fBodyAcc.meanFreq...Y<br>
</li>
<li>fBodyAcc.meanFreq...Z<br>
</li>
<li>fBodyAccJerk.mean...X<br>
</li>
<li>fBodyAccJerk.mean...Y<br>
</li>
<li>fBodyAccJerk.mean...Z</li>
<li>fBodyAccJerk.meanFreq...X<br>
</li>
<li>fBodyAccJerk.meanFreq...Y<br>
</li>
<li>fBodyAccJerk.meanFreq...Z<br>
</li>
<li>fBodyGyro.mean...X</li>
<li>fBodyGyro.mean...Y<br>
</li>
<li>fBodyGyro.mean...Z<br>
</li>
<li>fBodyGyro.meanFreq...X<br>
</li>
<li>fBodyGyro.meanFreq...Y<br>
</li>
<li>fBodyGyro.meanFreq...Z</li>
<li>fBodyAccMag.mean..</li>
<li>fBodyAccMag.meanFreq..</li>
<li>fBodyBodyAccJerkMag.mean..</li>
<li>fBodyBodyAccJerkMag.meanFreq..</li>
<li>fBodyBodyGyroMag.mean.. </li>
<li>fBodyBodyGyroMag.meanFreq.. </li>
<li>fBodyBodyGyroJerkMag.mean.. </li>
<li>fBodyBodyGyroJerkMag.meanFreq.. </li>
<li>tBodyAcc.std...X<br>
</li>
<li>tBodyAcc.std...Y<br>
</li>
<li>tBodyAcc.std...Z</li>
<li>tGravityAcc.std...X </li>
<li>tGravityAcc.std...Y </li>
<li>tGravityAcc.std...Z </li>
<li>tBodyAccJerk.std...X<br>
</li>
<li>tBodyAccJerk.std...Y</li>
<li>tBodyAccJerk.std...Z</li>
<li>tBodyGyro.std...X<br>
</li>
<li>tBodyGyro.std...Y<br>
</li>
<li>tBodyGyro.std...Z<br>
</li>
<li>tBodyGyroJerk.std...X<br>
</li>
<li>tBodyGyroJerk.std...Y<br>
</li>
<li>tBodyGyroJerk.std...Z<br>
</li>
<li>tBodyAccMag.std..<br>
</li>
<li>tGravityAccMag.std..</li>
<li>tBodyAccJerkMag.std..<br>
</li>
<li>tBodyGyroMag.std..</li>
<li>tBodyGyroJerkMag.std..</li>
<li>fBodyAcc.std...X<br>
</li>
<li>fBodyAcc.std...Y<br>
</li>
<li>fBodyAcc.std...Z<br>
</li>
<li>fBodyAccJerk.std...X</li>
<li>fBodyAccJerk.std...Y</li>
<li>fBodyAccJerk.std...Z<br>
</li>
<li>fBodyGyro.std...X<br>
</li>
<li>fBodyGyro.std...Y<br>
</li>
<li>fBodyGyro.std...Z<br>
</li>
<li>fBodyAccMag.std..<br>
</li>
<li>fBodyBodyAccJerkMag.std..</li>
<li>fBodyBodyGyroMag.std..</li>
<li>fBodyBodyGyroJerkMag.std..</li>
</ul>

<h1>
<a name="user-content-instructions" class="anchor" href="#instructions" aria-hidden="true"><span class="octicon octicon-link"></span></a>Instructions</h1>

<ul class="task-list">
<li>You can also get the feature instruction in the file features._info.txt in "UCI HAR Dataset" document</li>
</ul>

<p>The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 
Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 
Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). </p>

<p>These signals were used to estimate variables of the feature vector for each pattern:<br>
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.</p>

<ul class="task-list">
<li>tBodyAcc-XYZ</li>
<li>tGravityAcc-XYZ</li>
<li>tBodyAccJerk-XYZ</li>
<li>tBodyGyro-XYZ</li>
<li>tBodyGyroJerk-XYZ</li>
<li>tBodyAccMag</li>
<li>tGravityAccMag</li>
<li>tBodyAccJerkMag</li>
<li>tBodyGyroMag</li>
<li>tBodyGyroJerkMag</li>
<li>fBodyAcc-XYZ</li>
<li>fBodyAccJerk-XYZ</li>
<li>fBodyGyro-XYZ</li>
<li>fBodyAccMag</li>
<li>fBodyAccJerkMag</li>
<li>fBodyGyroMag</li>
<li>fBodyGyroJerkMag</li>
</ul>

<p>The set of variables that were estimated from these signals are: </p>

<ul class="task-list">
<li>mean(): Mean value</li>
<li>std(): Standard deviation</li>
<li>mad(): Median absolute deviation </li>
<li>max(): Largest value in array</li>
<li>min(): Smallest value in array</li>
<li>sma(): Signal magnitude area</li>
<li>energy(): Energy measure. Sum of the squares divided by the number of values. </li>
<li>iqr(): Interquartile range </li>
<li>entropy(): Signal entropy</li>
<li>arCoeff(): Autorregresion coefficients with Burg order equal to 4</li>
<li>correlation(): correlation coefficient between two signals</li>
<li>maxInds(): index of the frequency component with largest magnitude</li>
<li>meanFreq(): Weighted average of the frequency components to obtain a mean frequency</li>
<li>skewness(): skewness of the frequency domain signal </li>
<li>kurtosis(): kurtosis of the frequency domain signal </li>
<li>bandsEnergy(): Energy of a frequency interval within the 64 bins of the FFT of each window.</li>
<li>angle(): Angle between to vectors.</li>
</ul>

<p>Additional vectors obtained by averaging the signals in a signal window sample. These are used on the angle() variable:</p>

<ul class="task-list">
<li>gravityMean</li>
<li>tBodyAccMean</li>
<li>tBodyAccJerkMean</li>
<li>tBodyGyroMean</li>
<li>tBodyGyroJerkMean</li>
</ul>

<p>The complete list of variables of each feature vector is available in 'features.txt'</p>
</article>
  </div>

  </div>
</div>

<a href="#jump-to-line" rel="facebox[.linejump]" data-hotkey="l" style="display:none">Jump to Line</a>
<div id="jump-to-line" style="display:none">
  <form accept-charset="UTF-8" class="js-jump-to-line-form">
    <input class="linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" autofocus>
    <button type="submit" class="button">Go</button>
  </form>
</div>

        </div>

      </div><!-- /.repo-container -->
      <div class="modal-backdrop"></div>
    </div><!-- /.container -->
  </div><!-- /.site -->


    </div><!-- /.wrapper -->

      <div class="container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links right">
      <li><a href="https://status.github.com/">Status</a></li>
      <li><a href="https://developer.github.com">API</a></li>
      <li><a href="http://training.github.com">Training</a></li>
      <li><a href="http://shop.github.com">Shop</a></li>
      <li><a href="/blog">Blog</a></li>
      <li><a href="/about">About</a></li>

    </ul>

    <a href="/" aria-label="Homepage">
      <span class="mega-octicon octicon-mark-github" title="GitHub"></span>
    </a>

    <ul class="site-footer-links">
      <li>&copy; 2014 <span title="0.08481s from github-fe116-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="/site/terms">Terms</a></li>
        <li><a href="/site/privacy">Privacy</a></li>
        <li><a href="/security">Security</a></li>
        <li><a href="/contact">Contact</a></li>
    </ul>
  </div><!-- /.site-footer -->
</div><!-- /.container -->


    <div class="fullscreen-overlay js-fullscreen-overlay" id="fullscreen_overlay">
  <div class="fullscreen-container js-suggester-container">
    <div class="textarea-wrap">
      <textarea name="fullscreen-contents" id="fullscreen-contents" class="fullscreen-contents js-fullscreen-contents js-suggester-field" placeholder=""></textarea>
    </div>
  </div>
  <div class="fullscreen-sidebar">
    <a href="#" class="exit-fullscreen js-exit-fullscreen tooltipped tooltipped-w" aria-label="Exit Zen Mode">
      <span class="mega-octicon octicon-screen-normal"></span>
    </a>
    <a href="#" class="theme-switcher js-theme-switcher tooltipped tooltipped-w"
      aria-label="Switch themes">
      <span class="octicon octicon-color-mode"></span>
    </a>
  </div>
</div>



    <div id="ajax-error-message" class="flash flash-error">
      <span class="octicon octicon-alert"></span>
      <a href="#" class="octicon octicon-x flash-close js-ajax-error-dismiss" aria-label="Dismiss error"></a>
      Something went wrong with that request. Please try again.
    </div>


      <script crossorigin="anonymous" src="https://assets-cdn.github.com/assets/frameworks-dabc650f8a51dffd1d4376a3522cbda5536e4807e01d2a86ff7e60d8d6ee3029.js" type="text/javascript"></script>
      <script async="async" crossorigin="anonymous" src="https://assets-cdn.github.com/assets/github-d01013daa80c5a341ba3ddb684f2f26679eb369d67459151d5175a634a9e98a5.js" type="text/javascript"></script>
      
      
  </body>
</html>

