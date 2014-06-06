# FEM ("Free" Element Modifier)

##  The Free People UX Team CSS Naming Conventions

### Markup
    <form class="search-form">
        <fieldset>
            <label>Search:</label>
            <input type="search" class="search-form--input is-clicked" />
        </fieldset>
    </form>

### Conventions

1. **Parent Class Names:** train case for long class names (two or more words), ie, *.search-form*

2. **Child Class Names**: use two dashes to identify children of parent element, ie, *.search-form--input*

3. **Modifiers:** use train case for modifiers; the first word should be a verb, ie, *.search-form--input.is-clicked*

### SASS
    // parent element
    .search-form {
      margin: 0;
      padding: 0;
    }

    // child element of parent .search-form
    .search-form--input {
      background: #fff;
      padding: 3px;
      border: solid 1px #ccc;
      // modifier for child element .search-form--input
      &.is-clicked {
        border: solid 1px #ff0000;
      }
    }