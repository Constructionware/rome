# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `esprima > es2015-yield > invalid-yield-strict-arrow-parameter-name`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	filename: "esprima/es2015-yield/invalid-yield-strict-arrow-parameter-name/input.js"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "esprima/es2015-yield/invalid-yield-strict-arrow-parameter-name/input.js"
		end: Object {
			column: 0
			line: 2
		}
		start: Object {
			column: 0
			line: 1
		}
	}
	directives: Array [
		JSDirective {
			value: "use strict"
			loc: Object {
				filename: "esprima/es2015-yield/invalid-yield-strict-arrow-parameter-name/input.js"
				end: Object {
					column: 13
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
		}
	]
	diagnostics: Array [
		Object {
			origins: Array [Object {category: "parse/js"}]
			description: Object {
				advice: Array []
				category: "parse/js"
				message: MARKUP {
					parts: Array [
						"yield"
						RAW_MARKUP {value: " is a reserved word"}
					]
				}
			}
			location: Object {
				filename: "esprima/es2015-yield/invalid-yield-strict-arrow-parameter-name/input.js"
				mtime: undefined
				sourceText: undefined
				end: Object {
					column: 20
					line: 1
				}
				start: Object {
					column: 15
					line: 1
				}
			}
		}
	]
	body: Array [
		JSExpressionStatement {
			loc: Object {
				filename: "esprima/es2015-yield/invalid-yield-strict-arrow-parameter-name/input.js"
				end: Object {
					column: 27
					line: 1
				}
				start: Object {
					column: 14
					line: 1
				}
			}
			expression: JSArrowFunctionExpression {
				loc: Object {
					filename: "esprima/es2015-yield/invalid-yield-strict-arrow-parameter-name/input.js"
					end: Object {
						column: 27
						line: 1
					}
					start: Object {
						column: 14
						line: 1
					}
				}
				body: JSNumericLiteral {
					value: 42
					format: undefined
					loc: Object {
						filename: "esprima/es2015-yield/invalid-yield-strict-arrow-parameter-name/input.js"
						end: Object {
							column: 27
							line: 1
						}
						start: Object {
							column: 25
							line: 1
						}
					}
				}
				head: JSFunctionHead {
					async: false
					hasHoistedVars: false
					rest: undefined
					returnType: undefined
					thisType: undefined
					loc: Object {
						filename: "esprima/es2015-yield/invalid-yield-strict-arrow-parameter-name/input.js"
						end: Object {
							column: 24
							line: 1
						}
						start: Object {
							column: 14
							line: 1
						}
					}
					params: Array [
						JSBindingIdentifier {
							name: "yield"
							loc: Object {
								filename: "esprima/es2015-yield/invalid-yield-strict-arrow-parameter-name/input.js"
								identifierName: "yield"
								end: Object {
									column: 20
									line: 1
								}
								start: Object {
									column: 15
									line: 1
								}
							}
						}
					]
				}
			}
		}
	]
}
```

### `diagnostics`

```

 esprima/es2015-yield/invalid-yield-strict-arrow-parameter-name/input.js:1:15 parse/js ━━━━━━━━━━━━━

  ✖ yield is a reserved word

    "use strict"; (yield) => 42
                   ^^^^^

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```