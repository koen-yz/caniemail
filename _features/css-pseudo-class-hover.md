---
title: ":hover"
category: css
keywords: rollover, pseudo-class
last_test_date: "2019-10-23"
test_url: "/tests/css-selectors-pseudo-classes.html"
test_results_url: "https://app.emailonacid.com/app/acidtest/cl8ZYgIGE372fkVVuJkwNJDd7B4JUpo23Nz6qANcSlRUA/list"
stats: {
	apple-mail: {
		macos: {
			"12.4": "y" // YES pour :active, NOPE pour le reste
		},
		ios: {
			"12.1": "y",
            "13.1": "y" // NOPE pour le reste
		}
	},
	gmail: {
		desktop-webmail: {
			"2019-10": "y" // NOPE pour :active, :focus, :visited, :target
		},
		ios: {
			"2019-10": "n" // NOPE pour :active, :focus, :visited, :target
		},
		android: {
			"2019-10": "a #1" // NOPE pour :active, :focus, :visited, :target
		}
	},
    orange: {
        desktop-webmail: {
            "2019-10": "y" // OK pour :active, :focus, :visited, :target
        },
        ios: {
            "2019-10": "y" // NOPE pour :active, :focus, :visited, :target
        },
        android: {
            "2019-10": "y" // OK pour :active, :focus, :target | NOPE pour :visited
        }
    },
	outlook: {
		windows: {
			"2007": "n",
			"2010": "n",
			"2013": "n",
			"2016": "n",
			"2019": "n"
		},
		windows-10-mail: {
			"2019-10": "n"
		},
		macos: {
			"2019-02": "y"
		},
		outlook-com: {
			"2019-10": "a #2" // OK pour :active, :focus, :visited, :target (not filtered but does not work)
		},
		ios: {
			"2019-10": "n" // OK pour :target, NOPE pour le reste
		},
		android: {
			"2019-10": "y"
		}
	},
    thunderbird: {
        macos: {
            "60.8":"y" // OK pour tout
        }
    },
	yahoo: {
		desktop-webmail: {
			"2019-02": "y"
		},
		ios: {
			"2019-02": "y"
		},
		android: {
			"2019-02": "y"
		}
	},
	aol: {
		desktop-webmail: {
			"2019-02": "y"
		},
		ios: {
			"2019-02": "n"
		},
		android: {
			"2019-02": "y"
		}
	},
	samsung-email: {
		android: {
			"5.0.10.2": "y",
			"6.0.04.6": "y" // OK pour :focus, :target | NOPE pour :active, :visited
		}
	}
}
notes_by_num: {
	"1": "Partial. Not supported with non Gmail accounts.",
    "2": "Partial. Only supported on type selectors."
}
links: {
    "Can I use: :hover":"https://caniuse.com/#feat=mdn-css_selectors_hover",
    "MDN: :hover":"https://developer.mozilla.org/en-US/docs/Web/CSS/:hover"
}
---