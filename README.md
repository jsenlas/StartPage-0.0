<script>
  'use strict';

  var config = {
    categories: [

    /*
{ name: "", commands: [
        { key: '', name: '', url: '', search: '' },
        { key: '', name: '', url: '', search: '' },
        { key: '', name: '', url: '', search: '' },
        { key: '', name: '', url: '', search: '' },
        { key: '', name: '', url: '', search: '' },
      ] },


    */


      { name: "Social", commands: [
        { key: 'Fb', name: 'Facebook', url: 'https://www.facebook.com/', search: '' },
        { key: 'g', name: 'Gmail', url: 'https://gmail.com', search: '/#search/' },
        //{ key: '', name: '', url: '', search: '' },
        //{ key: '', name: '', url: '', search: '' },
      ] },
      { name: "VUT", commands: [
        { key: 'MSL', name: 'MyStudyLife', url: 'https://app.mystudylife.com/calendar', search: '' },
        { key: 'Rc', name: 'RoundCube', url: 'https://roundcube.fit.vutbr.cz/', search: '' },
        { key: 'W', name: 'Wis', url: 'https://wis.fit.vutbr.cz/FIT/', search: '' },
        { key: 'v', name: 'vutbr', url: 'https://www.vutbr.cz/', search: '' },
        { key: 'f', name: 'Fituska', url: 'https://fituska.eu/noauth.php', search: '' },
        { key: 'f', name: 'Fitator', url: 'https://fitator.cz/', search: '' },
        //{ key: '', name: '', url: '', search: '' },
        //{ key: '', name: '', url: '', search: '' },
      ] },
      { name: "Office", commands: [
        { key: 'L', name: 'Lingea', url: 'https://slovniky.lingea.sk/anglicko-slovensky', search: '' },
        //{ key: '', name: '', url: '', search: '' },
        //{ key: '', name: '', url: '', search: '' },
      ] },
      

      { name: "Nakup", commands: [
        { key: 'B', name: 'bazosSK', url: 'https://www.bazos.sk/', search: '' },
        { key: 'B', name: 'bazosCZ', url: 'https://www.bazos.cz/', search: '' },
        { key: 'Ls', name: 'Lionsport', url: 'https://www.lionsport.cz/', search: '' },
        { key: 'A', name: 'alzaSK', url: 'https://www.alza.sk/', search: '' },
        //{ key: '', name: '', url: '', search: '' },
        //{ key: '', name: '', url: '', search: '' },
      ] },
 

      { name: "Media", commands: [
        { key: 'y', name: 'YouTube', url: 'https://www.youtube.com', search: '/results?search_query=' },
        { key: 'Sc', name: 'Soundcloud', url: 'https://soundcloud.com/', search: '' },
        { key: 'd', name: 'Drive', url: 'https://drive.google.com/drive', search: '/search?q=' },
        { key: 'mu', name: 'Google Music', url: 'https://music.google.com', search: '/search?q=' },
        //{ key: '', name: '', url: '', search: '' },
        //{ key: '', name: '', url: '', search: '' },
      ] },
      { name: "Development", commands: [
        { key: 'gh', name: 'GitHub', url: 'https://github.com', search: '/search?q=' },
        //{ key: '', name: '', url: '', search: '' },
        //{ key: '', name: '', url: '', search: '' },
      ] },

      { name: "Tech", commands: [
        { key: 'Z', name: 'Zive', url: 'https://www.zive.cz/', search: '' },
        { key: 'Wcc', name: 'Wccftech', url: 'https://wccftech.com/', search: '' },        
        { key: 'Gsm', name: 'GsmArena', url: 'https://www.gsmarena.com/', search: '' },
        //{ key: '', name: '', url: '', search: '' },
        //{ key: '', name: '', url: '', search: '' },
      ] },
    ],


/* not used links
        { key: 't', name: 'Teknik', url: 'https://teknik.io' },
        { key: 'lo', name: 'Lobsters', url: 'https://lobste.rs/', search: '' }

      { name: "Indigo", commands: [
        { key: 'j', name: 'Jira', url: 'https://indigoca.atlassian.net/'},
        { key: 'c', name: 'Confluence', url: 'https://indigoca.atlassian.net/wiki/'},
        { key: 'b', name: 'Bitbucket', url: 'https://bitbucket.org/'},
        { key: 'al', name: 'Algolia', url: 'https://www.algolia.com/dashboard'},
        { key: 'az', name: 'Azure', url: 'https://portal.azure.com'},
        { key: 'oi', name: 'OurIndigo', url: 'https://www.ourindigo.ca/'},
        { key: 'n', name: 'NewRelic', url: 'https://insights.newrelic.com/'},
      ] },



*/


    // if none of the keys are matched, this is used for searching.
    defaultSearch: 'https://www.google.com/search?q=',

    // the delimiter between the key and your search query.
    // e.g. to search GitHub for potatoes you'd type "g:potatoes".
    searchDelimiter: ':',

    // the delimiter between the key and a path.
    // e.g. type "r/r/unixporn" to go to "reddit.com/r/unixporn".
    pathDelimiter: '/',

    // set to true to instantly redirect when a key is matched.
    // put a space before any search queries to prevent unwanted redirects.
    instantRedirect: false,

    // suggest your most popular queries as you type.
    suggestions: true,

    // max amount of suggestions to display.
    suggestionsLimit: 4,

    // open queries in a new tab.
    newTab: false,

    // the delimiter between the hours and minutes in the clock.
    clockDelimiter: ':',

    // used for determining when to redirect directly to a url.
    urlRegex: /^(?:(http|https)?:\/\/)?(?:[\w-]+\.)+([a-z]|[A-Z]|[0-9]){2,6}/i,

    // if "urlRegex" matches but this doesn't, "http://" will be
    // prepended to the beginning of the query before redirecting.
    protocolRegex: /^[a-zA-Z]+:\/\//i
  };
</script>

<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="robots" content="noindex">

<title>~</title>

<style type="text/css">
  @font-face {
    font-family: 'Lato';
    src: url('https://fonts.gstatic.com/s/lato/v11/22JRxvfANxSmnAhzbFH8PgLUuEpTyoUstqEm5AMlJo4.woff2') format('woff2');
  }

  body {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    margin: 0;
    padding: 0;
    color: white;
    background-color: #181818;
    font-family: 'Lato', sans-serif;
  }

  main {
    position: absolute;
    top: 35%;
    right: 0;
    left: 0;
    width: 90%;
    max-width: 310px;
    margin: 0 auto;
    transform: translateY(-100px);
    text-align: center;
  }

  time {
    display: block;
    margin-bottom: 20px;
    font-size: 5rem;
    letter-spacing: 6px;
  }

  input,
  input:focus {
    box-sizing: border-box;
    width: 100%;
    margin: 0;
    border: 0;
    background: #fff;
    outline: 0;
    -webkit-appearance: none;
    -moz-appearance: none;
    color: #0d0202;
    font-family: 'Lato', sans-serif;
  }

  ul,
  li {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .search-input {
    padding: 12px;
    border-radius: 2px;
    font-size: 1.1rem;
  }

  body[search-suggestions='true'] .search-input {
    border-radius: 2px 2px 0 0;
  }

  .search-suggestions {
    border-radius: 0 0 2px 2px;
    overflow: hidden;
  }

  .search-suggestion {
    padding: 14px 12px;
    transition: 0.5s;
    font-size: .8rem;
    cursor: pointer;
    text-align: left;
  }

  .search-suggestion:hover,
  .search-suggestion:focus {
    background: #30a388;
  }

  .overlay {
    position: relative;
    box-sizing: border-box;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    padding: 0 10px;
    transition: 200ms;
    background: #181818;
    visibility: visible;
    opacity: 1;
    overflow: auto;
  }

  .overlay[data-toggled='true'] {
    visibility: visible;
    opacity: 1;
  }

  .lists {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    padding-bottom: 20px;
    padding-top: 400px;
    overflow: auto;
  }

  .category {
    width: 160px;
    margin: 20px 10px 0;
  }

  .category-name {
    margin: 0;
    padding: 14px;
    border-radius: 2px 2px 0 0;
    background: #ab4642;
    color: #ffffff;
    font-size: .7rem;
    text-transform: uppercase;
    text-align: center;
  }

  .command {
    transition: background 200ms;
    background: #333;
  }

  .command:hover {
    background: #313131;
  }

  .command:nth-child(even) {
    background: #3a3a3a;
  }

  .command:nth-child(even):hover {
    background: #383838;
  }

  .command:last-of-type {
    border-radius: 0 0 2px 2px;
  }

  .command a {
    display: block;
    padding: 14px 12px;
    color: #eee;
    font-size: .8rem;
    line-height: 1.3rem;
    text-decoration: none;
  }

  .command-key {
    display: block;
    width: 32px;
    margin-right: 10px;
    float: left;
    border-radius: 2px;
    background: #292929;
    font-family: 'Courier New', monospace;
    text-align: center;
  }

  @media (min-width: 740px) {
    .overlay {
      display: inline;
      justify-content: center;
      align-items: center;
    }
  }
</style>

<aside id="js-overlay" class="overlay">
  <ul id="js-lists" class="lists"></ul>
</aside>

<main>
  <time id="js-clock"></time>
  <form id="js-search-form" autocomplete="off">
    <input id="js-search-input" class="search-input" type="text" autofocus>
    <ul id="js-search-suggestions" class="search-suggestions"></ul>
  </form>
</main>

<script>
  function $(s) {
    return document.querySelector(s);
  };

  var Clock = (function() {
    var clock = $('#js-clock');

    var pad = function(num) {
      return ('0' + num.toString()).slice(-2);
    }

    var setTime = function() {
      var date = new Date();
      var hours = pad(date.getHours());
      var minutes = pad(date.getMinutes());

      if (date.getSeconds() % 2) {
        clock.innerHTML = hours + config.clockDelimiter + minutes;
      } else {
        clock.innerHTML = hours + '<span style="opacity:0">' +  config.clockDelimiter + '</span>' + minutes;
      }
    }

    setTime();
    setInterval(setTime, 1000);
  })();

  var Help = (function() {
    var overlay = $('#js-overlay');
    var lists = $('#js-lists');

    config.categories.forEach(function(category) {
      var commandItems = '';

      category.commands.forEach(function(command) {
        commandItems += (
          '<li class="command">' +
            '<a href="' + command.url + '">' +
              '<span class="command-key">' + command.key + '</span>' +
              '<span class="command-name">' + command.name + '</span>' +
            '</a>' +
          '</li>'
        );
      });

      lists.insertAdjacentHTML(
        'beforeend',
        '<li class="category">' +
          '<h2 class="category-name">' + category.name + '</h2>' +
          '<ul>' + commandItems + '</ul>' +
        '</li>'
      );
    });

    return {
      toggle: function(show) {
        var toggle = typeof show !== 'undefined' ? show :
          overlay.getAttribute('data-toggled') !== 'true';

        overlay.setAttribute('data-toggled', toggle);
      }
    };
  })();

  var Suggestions = (function() {
    var searchSuggestions = $('#js-search-suggestions');
    var queries = JSON.parse(localStorage.getItem('queries')) || [];

    return {
      add: function(q) {
        if (q.length < 2) return;

        var exists = false;

        queries.forEach(function(query) {
          if (query[0] === q) {
            query[1]++;
            exists = true;
          }
        });

        if (!exists) queries.push([q, 1]);

        queries = queries.sort(function(current, next) {
          return current[1] > next[1];
        }).reverse();

        localStorage.setItem('queries', JSON.stringify(queries));
      },

      show: function(input) {
        searchSuggestions.innerHTML = '';
        document.body.setAttribute('search-suggestions', false);

        if (!config.suggestions || !input) return false;

        queries
          .filter(function(query) {
            var matchesQuery = query[0].indexOf(input) !== -1;
            return input && matchesQuery && input !== query[0];
          })
          .slice(0, config.suggestionsLimit).forEach(function(query) {
            searchSuggestions.insertAdjacentHTML(
              'beforeend',
              '<li>' +
                '<input ' +
                  'class="search-suggestion"' +
                  'type="button" ' +
                  'onclick="Form.submitWithThis.call(this)"' +
                  'value="' + query[0] + '"' +
                '>' +
              '</li>'
            );

            document.body.setAttribute('search-suggestions', true)
          });
      }
    };
  })();

  var Form = (function() {
    var searchForm = $('#js-search-form');
    var searchInput = $('#js-search-input');

    var execute = function(query, redirect) {
      Suggestions.add(query);
      Suggestions.show('');
      searchInput.value = '';

      if (config.newTab) window.open(redirect, '_blank');
      else window.location.href = redirect;
    }

    var keyPress = function(event) {
      var char = String.fromCharCode(event.which);

      if (char.length && event.which !== 13) {
        Help.toggle(false);
        searchInput.focus();
      }

      if (config.instantRedirect) {
        config.categories.forEach(function(category) {
          category.commands.forEach(function(command) {
            var query = searchInput.value + char;

            if (command.key === query) {
              event.preventDefault();
              execute(query, command.url);
            }
          });
        });
      }
    };

    var submit = function(event) {
      if (event) event.preventDefault();

      var q = searchInput.value.trim();

      if (!q) {
        Help.toggle();
        return false;
      }

      var qSplitSearch = q.split(config.searchDelimiter);
      var qSplitPath = q.split(config.pathDelimiter);
      var qIsUrl = q.match(config.urlRegex);
      var qHasProtocol = q.match(config.protocolRegex);
      var redirect = '';
      var breakLoop = false;

      if (qIsUrl) redirect = qHasProtocol ? q : 'http://' + q;
      else redirect = config.defaultSearch + encodeURIComponent(q);

      config.categories.forEach(function(category) {
        category.commands.forEach(function(command) {
          var isSearch = qSplitSearch[0] === command.key;
          var isPath = qSplitPath[0] === command.key;

          if (isSearch || isPath) {
            if (qSplitSearch[1] && command.search) {
              qSplitSearch.shift();

              var search = encodeURIComponent(
                qSplitSearch.join(config.searchDelimiter).trim()
              );

              redirect = command.url + command.search + search;
            } else if (qSplitPath[1]) {
              qSplitPath.shift();
              var path = qSplitPath.join(config.pathDelimiter).trim();
              redirect = command.url + '/' + path;
            } else {
              redirect = command.url;
            }

            breakLoop = true;
            return;
          }
        });

        if (breakLoop) return;
      });

      execute(q, redirect);
    }

    var keyUp = function(event) {
      Suggestions.show(searchInput.value.trim());
    }

    document.addEventListener('keypress', keyPress);
    searchForm.addEventListener('submit', submit, false);
    searchInput.addEventListener('keyup', keyUp);

    return {
      submitWithThis: function() {
        searchInput.value = this.value;
        submit();
      }
    };
  })();

  $("div").removeClass("container-lg");
</script>
