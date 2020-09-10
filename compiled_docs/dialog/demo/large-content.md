{"title":"内容较多的对话框","meta":{"title":"内容较多的对话框","description":"\n","order":"4"},"codes":{"jsx":"import { Switch, Button, Dialog } from '@alifd/next';\n\n\nconst largeContent = new Array(30).fill(\n    <p>Start your business here by searching a popular product</p>\n);\n\nclass Demo extends React.Component {\n    state = {\n        visible: false,\n        isFullScreen: false,\n        closeOnMaskClick: false,\n    };\n\n    onOpen = () => {\n        this.setState({\n            visible: true\n        });\n    };\n\n    onClose = () => {\n        this.setState({\n            visible: false\n        });\n    };\n\n    toggleIsFullScreen = () => {\n        this.setState({\n            isFullScreen: !this.state.isFullScreen\n        });\n    }\n\n    toggleCloseOnMaskClick = () => {\n        this.setState({\n            closeOnMaskClick: !this.state.closeOnMaskClick\n        });\n    }\n\n    render() {\n        const { visible, isFullScreen, closeOnMaskClick } = this.state;\n\n        return (\n            <div>\n                <div style={{ display: 'block', marginBottom: '10px' }}>\n                    When the height of the dialog exceeds the viewport height of the browser, whether to show the scroll bar:\n                </div>\n                <Switch style={{ display: 'block', marginBottom: '10px' }} checked={isFullScreen} onChange={this.toggleIsFullScreen} />\n                <div style={{ display: 'block', marginBottom: '10px' }}>\n                    Close on mask click:\n                </div>\n                <Switch style={{ display: 'block', marginBottom: '10px' }} checked={closeOnMaskClick} onChange={this.toggleCloseOnMaskClick} />\n                <Button onClick={this.onOpen} type=\"primary\">\n                    Open dialog\n                </Button>\n                <Dialog title=\"Welcome to Alibaba.com\"\n                    visible={visible}\n                    isFullScreen={isFullScreen}\n                    closeable={closeOnMaskClick ? 'close,esc,mask' : 'close,esc'}\n                    onOk={this.onClose}\n                    onCancel={this.onClose}\n                    onClose={this.onClose}>\n                    {largeContent}\n                </Dialog>\n            </div>\n        );\n    }\n}\n\nReactDOM.render(<Demo />, mountNode);\n"},"body":"\n\n````jsx\nimport { Switch, Button, Dialog } from '@alifd/next';\n\n\nconst largeContent = new Array(30).fill(\n    <p>Start your business here by searching a popular product</p>\n);\n\nclass Demo extends React.Component {\n    state = {\n        visible: false,\n        isFullScreen: false,\n        closeOnMaskClick: false,\n    };\n\n    onOpen = () => {\n        this.setState({\n            visible: true\n        });\n    };\n\n    onClose = () => {\n        this.setState({\n            visible: false\n        });\n    };\n\n    toggleIsFullScreen = () => {\n        this.setState({\n            isFullScreen: !this.state.isFullScreen\n        });\n    }\n\n    toggleCloseOnMaskClick = () => {\n        this.setState({\n            closeOnMaskClick: !this.state.closeOnMaskClick\n        });\n    }\n\n    render() {\n        const { visible, isFullScreen, closeOnMaskClick } = this.state;\n\n        return (\n            <div>\n                <div style={{ display: 'block', marginBottom: '10px' }}>\n                    When the height of the dialog exceeds the viewport height of the browser, whether to show the scroll bar:\n                </div>\n                <Switch style={{ display: 'block', marginBottom: '10px' }} checked={isFullScreen} onChange={this.toggleIsFullScreen} />\n                <div style={{ display: 'block', marginBottom: '10px' }}>\n                    Close on mask click:\n                </div>\n                <Switch style={{ display: 'block', marginBottom: '10px' }} checked={closeOnMaskClick} onChange={this.toggleCloseOnMaskClick} />\n                <Button onClick={this.onOpen} type=\"primary\">\n                    Open dialog\n                </Button>\n                <Dialog title=\"Welcome to Alibaba.com\"\n                    visible={visible}\n                    isFullScreen={isFullScreen}\n                    closeable={closeOnMaskClick ? 'close,esc,mask' : 'close,esc'}\n                    onOk={this.onClose}\n                    onCancel={this.onClose}\n                    onClose={this.onClose}>\n                    {largeContent}\n                </Dialog>\n            </div>\n        );\n    }\n}\n\nReactDOM.render(<Demo />, mountNode);\n````","html":"<script>(function(){'use strict';\n\nvar _createClass = function () { function defineProperties(target, props) { for (var i = 0; i < props.length; i++) { var descriptor = props[i]; descriptor.enumerable = descriptor.enumerable || false; descriptor.configurable = true; if (\"value\" in descriptor) descriptor.writable = true; Object.defineProperty(target, descriptor.key, descriptor); } } return function (Constructor, protoProps, staticProps) { if (protoProps) defineProperties(Constructor.prototype, protoProps); if (staticProps) defineProperties(Constructor, staticProps); return Constructor; }; }();\n\nvar _next = require('@alifd/next');\n\nfunction _classCallCheck(instance, Constructor) { if (!(instance instanceof Constructor)) { throw new TypeError(\"Cannot call a class as a function\"); } }\n\nfunction _possibleConstructorReturn(self, call) { if (!self) { throw new ReferenceError(\"this hasn't been initialised - super() hasn't been called\"); } return call && (typeof call === \"object\" || typeof call === \"function\") ? call : self; }\n\nfunction _inherits(subClass, superClass) { if (typeof superClass !== \"function\" && superClass !== null) { throw new TypeError(\"Super expression must either be null or a function, not \" + typeof superClass); } subClass.prototype = Object.create(superClass && superClass.prototype, { constructor: { value: subClass, enumerable: false, writable: true, configurable: true } }); if (superClass) Object.setPrototypeOf ? Object.setPrototypeOf(subClass, superClass) : subClass.__proto__ = superClass; }\n\nvar largeContent = new Array(30).fill(React.createElement(\n    'p',\n    null,\n    'Start your business here by searching a popular product'\n));\n\nvar Demo = function (_React$Component) {\n    _inherits(Demo, _React$Component);\n\n    function Demo() {\n        var _ref;\n\n        var _temp, _this, _ret;\n\n        _classCallCheck(this, Demo);\n\n        for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {\n            args[_key] = arguments[_key];\n        }\n\n        return _ret = (_temp = (_this = _possibleConstructorReturn(this, (_ref = Demo.__proto__ || Object.getPrototypeOf(Demo)).call.apply(_ref, [this].concat(args))), _this), _this.state = {\n            visible: false,\n            isFullScreen: false,\n            closeOnMaskClick: false\n        }, _this.onOpen = function () {\n            _this.setState({\n                visible: true\n            });\n        }, _this.onClose = function () {\n            _this.setState({\n                visible: false\n            });\n        }, _this.toggleIsFullScreen = function () {\n            _this.setState({\n                isFullScreen: !_this.state.isFullScreen\n            });\n        }, _this.toggleCloseOnMaskClick = function () {\n            _this.setState({\n                closeOnMaskClick: !_this.state.closeOnMaskClick\n            });\n        }, _temp), _possibleConstructorReturn(_this, _ret);\n    }\n\n    _createClass(Demo, [{\n        key: 'render',\n        value: function render() {\n            var _state = this.state,\n                visible = _state.visible,\n                isFullScreen = _state.isFullScreen,\n                closeOnMaskClick = _state.closeOnMaskClick;\n\n\n            return React.createElement(\n                'div',\n                null,\n                React.createElement(\n                    'div',\n                    { style: { display: 'block', marginBottom: '10px' } },\n                    'When the height of the dialog exceeds the viewport height of the browser, whether to show the scroll bar:'\n                ),\n                React.createElement(_next.Switch, { style: { display: 'block', marginBottom: '10px' }, checked: isFullScreen, onChange: this.toggleIsFullScreen }),\n                React.createElement(\n                    'div',\n                    { style: { display: 'block', marginBottom: '10px' } },\n                    'Close on mask click:'\n                ),\n                React.createElement(_next.Switch, { style: { display: 'block', marginBottom: '10px' }, checked: closeOnMaskClick, onChange: this.toggleCloseOnMaskClick }),\n                React.createElement(\n                    _next.Button,\n                    { onClick: this.onOpen, type: 'primary' },\n                    'Open dialog'\n                ),\n                React.createElement(\n                    _next.Dialog,\n                    { title: 'Welcome to Alibaba.com',\n                        visible: visible,\n                        isFullScreen: isFullScreen,\n                        closeable: closeOnMaskClick ? 'close,esc,mask' : 'close,esc',\n                        onOk: this.onClose,\n                        onCancel: this.onClose,\n                        onClose: this.onClose },\n                    largeContent\n                )\n            );\n        }\n    }]);\n\n    return Demo;\n}(React.Component);\n\nReactDOM.render(React.createElement(Demo, null), mountNode);})()</script><div class=\"highlight\"><pre class=\"language-jsx\"><code class=\"language-jsx\"><span class=\"token keyword\">import</span> <span class=\"token punctuation\">{</span> Switch<span class=\"token punctuation\">,</span> Button<span class=\"token punctuation\">,</span> Dialog <span class=\"token punctuation\">}</span> <span class=\"token keyword\">from</span> <span class=\"token string\">'@alifd/next'</span><span class=\"token punctuation\">;</span>\n\n\n<span class=\"token keyword\">const</span> largeContent <span class=\"token operator\">=</span> <span class=\"token keyword\">new</span> <span class=\"token class-name\">Array</span><span class=\"token punctuation\">(</span><span class=\"token number\">30</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">.</span><span class=\"token function\">fill</span><span class=\"token punctuation\">(</span>\n    <span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>p</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">Start your business here by searching a popular product</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>p</span><span class=\"token punctuation\">></span></span>\n<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n\n<span class=\"token keyword\">class</span> <span class=\"token class-name\">Demo</span> <span class=\"token keyword\">extends</span> <span class=\"token class-name\">React<span class=\"token punctuation\">.</span>Component</span> <span class=\"token punctuation\">{</span>\n    state <span class=\"token operator\">=</span> <span class=\"token punctuation\">{</span>\n        visible<span class=\"token operator\">:</span> <span class=\"token boolean\">false</span><span class=\"token punctuation\">,</span>\n        isFullScreen<span class=\"token operator\">:</span> <span class=\"token boolean\">false</span><span class=\"token punctuation\">,</span>\n        closeOnMaskClick<span class=\"token operator\">:</span> <span class=\"token boolean\">false</span><span class=\"token punctuation\">,</span>\n    <span class=\"token punctuation\">}</span><span class=\"token punctuation\">;</span>\n\n    <span class=\"token function-variable function\">onOpen</span> <span class=\"token operator\">=</span> <span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\n        <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span><span class=\"token function\">setState</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">{</span>\n            visible<span class=\"token operator\">:</span> <span class=\"token boolean\">true</span>\n        <span class=\"token punctuation\">}</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span><span class=\"token punctuation\">;</span>\n\n    <span class=\"token function-variable function\">onClose</span> <span class=\"token operator\">=</span> <span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\n        <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span><span class=\"token function\">setState</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">{</span>\n            visible<span class=\"token operator\">:</span> <span class=\"token boolean\">false</span>\n        <span class=\"token punctuation\">}</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span><span class=\"token punctuation\">;</span>\n\n    <span class=\"token function-variable function\">toggleIsFullScreen</span> <span class=\"token operator\">=</span> <span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\n        <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span><span class=\"token function\">setState</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">{</span>\n            isFullScreen<span class=\"token operator\">:</span> <span class=\"token operator\">!</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>state<span class=\"token punctuation\">.</span>isFullScreen\n        <span class=\"token punctuation\">}</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n\n    <span class=\"token function-variable function\">toggleCloseOnMaskClick</span> <span class=\"token operator\">=</span> <span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\n        <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span><span class=\"token function\">setState</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">{</span>\n            closeOnMaskClick<span class=\"token operator\">:</span> <span class=\"token operator\">!</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>state<span class=\"token punctuation\">.</span>closeOnMaskClick\n        <span class=\"token punctuation\">}</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n\n    <span class=\"token function\">render</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n        <span class=\"token keyword\">const</span> <span class=\"token punctuation\">{</span> visible<span class=\"token punctuation\">,</span> isFullScreen<span class=\"token punctuation\">,</span> closeOnMaskClick <span class=\"token punctuation\">}</span> <span class=\"token operator\">=</span> <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>state<span class=\"token punctuation\">;</span>\n\n        <span class=\"token keyword\">return</span> <span class=\"token punctuation\">(</span>\n            <span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>div</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>div</span> <span class=\"token attr-name\">style</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">{</span> display<span class=\"token operator\">:</span> <span class=\"token string\">'block'</span><span class=\"token punctuation\">,</span> marginBottom<span class=\"token operator\">:</span> <span class=\"token string\">'10px'</span> <span class=\"token punctuation\">}</span><span class=\"token punctuation\">}</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                    When the height of the dialog exceeds the viewport height of the browser, whether to show the scroll bar:\n                </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>div</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Switch</span></span> <span class=\"token attr-name\">style</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">{</span> display<span class=\"token operator\">:</span> <span class=\"token string\">'block'</span><span class=\"token punctuation\">,</span> marginBottom<span class=\"token operator\">:</span> <span class=\"token string\">'10px'</span> <span class=\"token punctuation\">}</span><span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">checked</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span>isFullScreen<span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">onChange</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>toggleIsFullScreen<span class=\"token punctuation\">}</span></span> <span class=\"token punctuation\">/></span></span><span class=\"token plain-text\">\n                </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>div</span> <span class=\"token attr-name\">style</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">{</span> display<span class=\"token operator\">:</span> <span class=\"token string\">'block'</span><span class=\"token punctuation\">,</span> marginBottom<span class=\"token operator\">:</span> <span class=\"token string\">'10px'</span> <span class=\"token punctuation\">}</span><span class=\"token punctuation\">}</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                    Close on mask click:\n                </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>div</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Switch</span></span> <span class=\"token attr-name\">style</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">{</span> display<span class=\"token operator\">:</span> <span class=\"token string\">'block'</span><span class=\"token punctuation\">,</span> marginBottom<span class=\"token operator\">:</span> <span class=\"token string\">'10px'</span> <span class=\"token punctuation\">}</span><span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">checked</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span>closeOnMaskClick<span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">onChange</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>toggleCloseOnMaskClick<span class=\"token punctuation\">}</span></span> <span class=\"token punctuation\">/></span></span><span class=\"token plain-text\">\n                </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Button</span></span> <span class=\"token attr-name\">onClick</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>onOpen<span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">type</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>primary<span class=\"token punctuation\">\"</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                    Open dialog\n                </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span><span class=\"token class-name\">Button</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Dialog</span></span> <span class=\"token attr-name\">title</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>Welcome to Alibaba.com<span class=\"token punctuation\">\"</span></span>\n                    <span class=\"token attr-name\">visible</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span>visible<span class=\"token punctuation\">}</span></span>\n                    <span class=\"token attr-name\">isFullScreen</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span>isFullScreen<span class=\"token punctuation\">}</span></span>\n                    <span class=\"token attr-name\">closeable</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span>closeOnMaskClick <span class=\"token operator\">?</span> <span class=\"token string\">'close,esc,mask'</span> <span class=\"token operator\">:</span> <span class=\"token string\">'close,esc'</span><span class=\"token punctuation\">}</span></span>\n                    <span class=\"token attr-name\">onOk</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>onClose<span class=\"token punctuation\">}</span></span>\n                    <span class=\"token attr-name\">onCancel</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>onClose<span class=\"token punctuation\">}</span></span>\n                    <span class=\"token attr-name\">onClose</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>onClose<span class=\"token punctuation\">}</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                    </span><span class=\"token punctuation\">{</span>largeContent<span class=\"token punctuation\">}</span><span class=\"token plain-text\">\n                </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span><span class=\"token class-name\">Dialog</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n            </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>div</span><span class=\"token punctuation\">></span></span>\n        <span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n<span class=\"token punctuation\">}</span>\n\nReactDOM<span class=\"token punctuation\">.</span><span class=\"token function\">render</span><span class=\"token punctuation\">(</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Demo</span></span> <span class=\"token punctuation\">/></span></span><span class=\"token punctuation\">,</span> mountNode<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span></code></pre></div>"}