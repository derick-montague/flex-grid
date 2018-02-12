# flex-grid
A simple grid built with LESS and flexbox

```
@bp-min: 320px;
@bp-xs: 480px;
@bp-sm: 540px;
@bp-med: 768px;
@bp-lg: 990px;
@bp-xl: 1240px;
@bp-xxl: 1440px;
@bp-max: 1920px;

.flex-row(@size: @bp-med) {
  @media (min-width: @size) {
    
    > * {
      flex: auto;
    }
    
    .l-flex__eighth {
      flex: 0 0 12.5%;
    }
    
    .l-flex__quarter {
      flex: 0 0 25%;
    }
    
    .l-flex__third {
      flex: 0 0 33.333%;
    }
    
    .l-flex__half {
      flex: 0 0 50%;
    }
    
    .l-flex__two-third {
      flex: 0 0 66.666%;
    }
    
    .l-flex__three-quarter {
      flex: 0 0 75%;
    }
    
    .l-flex__full {
      flex: 0 0 100%;
    }
  }
}

.l-flex {
    display: flex;
    flex-wrap: wrap;
    margin-left: -.5rem;
    margin-top: -.5rem;
    margin-bottom: .5rem;

    > * {
        box-sizing: border-box;
        flex:  0 0 100%;
        padding-left: .5rem;
        padding-top: .5rem;
    }

    &.l-flex--no-row-gap {
        margin-top: 0;
        margin-bottom: 0;

        > * {
            padding-top: 0;
        }
    }

    &.l-flex--no-col-gap {
        margin-left: 0;
      
        > * {
            padding-left: 0;
        }
    }

    &.l-flex--no-gap {
        .l-flex--no-row-gap;
        .l-flex--no-col-gap;
    }
}

.l-flex--row-min {
  .flex-row(@bp-min);
}

.l-flex--row-xs {
  .flex-row(@bp-xs);
}

.l-flex--row-sm {
  .flex-row(@bp-sm);
}

.l-flex--row-med {
  .flex-row(@bp-med);
}

.l-flex--row-lg {
  .flex-row(@bp-lg);
}

.l-flex--row-xl {
  .flex-row(@bp-xl);
}

.l-flex--row-xxl {
  .flex-row(@bp-xxl);
}

.l-flex--row-max {
  .flex-row(@bp-max);
}
```
